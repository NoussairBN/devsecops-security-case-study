# Validation et qualité des résultats

## États utilisés

| État | Signification |
|---|---|
| `PASS` | Le comportement attendu a été observé |
| `FAIL` | Un critère de sécurité obligatoire n'est pas satisfait |
| `WARN` | Le résultat nécessite une analyse humaine |
| `SKIP` | Les préconditions du scénario ne sont pas disponibles |
| Erreur | Le test n'a pas pu s'exécuter correctement |

Cette taxonomie évite qu'une erreur technique soit assimilée à un système
sécurisé ou qu'un avertissement soit présenté comme une vulnérabilité prouvée.

## Revalidation croisée

Pour les contrôles d'autorisation, la validation doit utiliser au minimum deux
profils :

1. un profil non autorisé, qui doit recevoir un refus sans modification de
   l'état ;
2. un profil légitime, qui doit conserver l'opération métier prévue.

## Interprétation prudente

Le résultat final d'une pipeline correspond à l'état des scénarios couverts au
moment de l'exécution. Il ne démontre pas l'absence absolue de vulnérabilité.
Les limites de périmètre, les avertissements, les dépendances et les risques de
chaîne logicielle restent à surveiller.

## Améliorations possibles

- ajouter des tests unitaires et d'intégration des règles d'autorisation ;
- isoler l'état de chaque scénario dynamique ;
- conserver des rapports structurés comme artefacts ;
- épingler les actions tierces sur des références immuables ;
- générer un SBOM ;
- signer les images et attestations de provenance ;
- centraliser les événements de sécurité et définir des délais de traitement.

