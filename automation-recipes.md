# Retete de automatizari pentru Apex Move
Spune-i lui Robert "creeaza agent X" pe baza acestor idei:
1. MONITOR-STOC: worker cu cron care citeste un Google Sheet cu stocuri si trimite alerta pe Telegram cand un produs < 5 buc.
2. URMARITOR-PRET-CONCURENTI: cron zilnic, fetch pe paginile a 3 concurenti, extrage pretul cu regex, salveaza in KV, alerteaza la scaderi.
3. COLECTOR-COMENZI: webhook care primeste comenzi (de pe site/form), le scrie intr-un Sheet/D1 si confirma pe Telegram.
4. RAPORT-ZILNIC: cron 20:00 care aduna vanzarile zilei din KV si trimite un rezumat.
5. RASPUNS-AUTOMAT-DM: bot care raspunde la intrebari frecvente (marimi, livrare) din KV.
