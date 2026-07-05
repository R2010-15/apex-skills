# Cum sa scrii prompturi bune pentru Groq/AI
1. Da ROL clar: "Esti expert in X".
2. Cere FORMAT exact: "Raspunde DOAR cu JSON: {...}" + response_format:{type:'json_object'}.
3. Da EXEMPLE (1-2) de intrare->iesire.
4. Limiteaza: "maxim 3 propozitii", "in romana".
5. Context relevant, nu tot. temperature 0.3 precizie / 0.9 creativitate.
6. Sarcini lungi -> imparte in pasi. Ajusteaza promptul, nu modelul.
