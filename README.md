# Stratégie 2027

Questionnaire interne, protégé par phrase de passe.

`index.html` est chiffré (AES-256-GCM, clé dérivée en PBKDF2-HMAC-SHA256,
600 000 itérations). Sans la phrase de passe, la page n'expose aucun contenu.

Le déchiffrement utilise WebCrypto et exige une origine sécurisée : la page
doit être servie en https.

Les sources et l'outil de compilation ne sont pas versionnés ici.
