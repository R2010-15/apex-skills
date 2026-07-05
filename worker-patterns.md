# Pattern-uri Cloudflare Workers pentru agenti robusti
1. RETRY cu backoff: for(let i=0;i<3;i++){const r=await fetch(...); if(r.ok)break; await new Promise(s=>setTimeout(s,1000*(i+1)));}
2. CACHE in KV cu TTL: env.KV.put(k,v,{expirationTtl:3600}).
3. Raspuns rapid la webhook + lucru in fundal: ctx.waitUntil(taskLunga()).
4. Rate limit simplu: contor in KV pe fereastra de timp.
5. Cozi (Queues) pentru sarcini multe. Durable Objects pentru stare partajata.
Mereu try/catch la fetch extern.
