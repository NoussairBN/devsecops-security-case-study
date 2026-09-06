# Méthodologie d'audit

## Référentiels

La démarche s'est inspirée de PTES pour l'organisation générale du test,
d'OWASP WSTG pour les familles de vérifications web, d'OWASP API Security pour
les risques propres aux API et de CVSS pour assister la priorisation.

## Étapes

### 1. Cadrage

Identification des actifs autorisés, des profils de test, des limites
opérationnelles et des critères de preuve.

### 2. Reconnaissance maîtrisée

Inventaire des composants visibles et vérification de la surface exposée, sans
publier ici les domaines, adresses, versions ou services observés.

### 3. Tests black box

Évaluation des fonctions accessibles sans connaissance du code : exposition
d'informations, authentification, limitation de débit et configuration HTTP.

### 4. Tests grey box

Utilisation de plusieurs profils autorisés pour vérifier la matrice
rôle–ressource–action : lecture, création, modification et administration.

### 5. Qualification

Chaque observation a été classée selon sa reproductibilité, ses préconditions,
son impact technique, son impact métier et la confiance dans la preuve.

### 6. Revalidation

Le scénario initial a été rejoué après correction. Un test positif a également
été conservé lorsque cela était nécessaire pour vérifier que le comportement
métier légitime n'avait pas été cassé.

## Principes de preuve

- une réponse HTTP positive ne suffit pas toujours à démontrer un impact ;
- une valeur réfléchie doit être distinguée d'un changement réellement
  persistant ;
- un statut vert de pipeline ne remplace pas l'analyse de ses journaux ;
- un avertissement n'est pas automatiquement une vulnérabilité ;
- une erreur d'environnement ne doit jamais être interprétée comme un succès de
  sécurité.

