# Contexte et cadrage

## Contexte général

La mission concernait une application web interne manipulant des identités,
des rôles et des processus métier. L'objectif n'était pas seulement de produire
une liste de constats, mais de construire une boucle durable reliant audit,
correction et prévention des régressions.

Le contenu public reste volontairement indépendant de l'organisation et du
produit concernés. Les technologies, flux et actifs sont décrits uniquement au
niveau nécessaire pour expliquer la démarche professionnelle.

## Problématique

> Comment identifier, traiter et prévenir les vulnérabilités d'une application
> web existante tout en intégrant des contrôles de sécurité reproductibles dans
> son cycle de développement ?

## Périmètre méthodologique

La démarche a porté sur :

- l'interface web et son API ;
- les mécanismes d'authentification et d'autorisation ;
- les dépendances logicielles ;
- la configuration des services nécessaires au développement ;
- les mécanismes de livraison et de validation automatisée.

## Règles d'engagement

- utilisation exclusive de comptes et environnements autorisés ;
- exclusion des attaques destructrices et du déni de service volumétrique ;
- maîtrise du volume et de la fréquence des requêtes ;
- recours à des données synthétiques ou de test ;
- conservation séparée des preuves confidentielles ;
- validation manuelle avant de qualifier un résultat automatisé.

## Critères de réussite

Une amélioration était considérée comme démontrée lorsque le scénario initial
n'était plus reproductible, que l'état métier restait cohérent et que l'usage
légitime demeurait disponible. Les scénarios prioritaires devaient ensuite être
transformés en contrôles de non-régression automatisables.

