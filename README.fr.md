[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Console de gouvernance des stocks DTC transfrontalière
## Nettoyage des signaux de demande, maîtrise des engagements de précommande et planification des achats pour les marques Shopify

![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Browser%20%7C%20Excel-success)
![Tool](https://img.shields.io/badge/Tool-Inventory%20Decision%20Support-orange)

**Transformez des données de commandes Shopify bruyantes en décisions d'achat en quelques minutes—directement dans le navigateur ou dans le classeur Excel, sans inscription, sans installation et sans abonnement récurrent.**

**Pas d'inscription. Pas d'installation. Gratuit dans votre navigateur.**

Essayez la version navigateur gratuitement. Si vous avez besoin de la version Excel, vous pouvez l'acheter avec une garantie de remboursement de 30 jours sans question.
>
> 🌐 **Ouvrir dans le navigateur** → [*Version HTML en ligne*](https://hyvoid.github.io/Cross-Border-DTC-Inventory-Governance-Console/)
>
> 📥 **Télécharger la version Excel**  
> *(Publication GitHub / téléchargement depuis le [Site web](https://www.theseusworkshop.com/))*

---

## Ce que cet outil vous aide à suivre

Au lieu de consulter des rapports déconnectés issus de Shopify, d'Inventory Planner et de feuilles de calcul, cette console réunit les signaux opérationnels dans un cadre décisionnel unique.

Elle permet de voir :

- Les engagements de précommande en cours qui ne doivent pas être comptés comme du stock disponible.
- La demande réelle après suppression de la distorsion liée aux précommandes et des retours attendus.
- Les quantités d'achat qui reflètent les obligations de stock réelles au lieu de ventes gonflées.
- La répartition des stocks entre le Royaume-Uni, les États-Unis, l'UE et l'Australie selon la contribution de la demande.
- Les écarts de synchronisation entre Shopify, Inventory Planner et les registres d'achats avant qu'ils ne deviennent des erreurs de planification.
- Les priorités d'achat hebdomadaires appuyées sur des données opérationnelles rapprochées plutôt que sur des ajustements manuels de feuilles de calcul.

---

## Flux de travail de démarrage rapide

Le classeur est conçu autour d'un flux de travail **configurer une fois, actualiser régulièrement** plutôt que d'une maintenance constante des feuilles de calcul.

### 1. Configurer les paramètres opérationnels

Ouvrez la feuille **Config** et définissez les règles opérationnelles telles que :

- le délai d'approvisionnement
- la fenêtre de retour
- le ratio de répartition des marchés
- le facteur de sécurité des précommandes

Ces valeurs ne changent généralement que lorsque les politiques métier évoluent.

---

### 2. Importer les données métier existantes

Exportez vos données opérationnelles existantes depuis Shopify et Inventory Planner.

Collez ou actualisez :

- Shopify Orders
- Shopify Returns
- Current Inventory
- Purchase Status

Aucune restructuration ni mise à jour manuelle des formules n'est requise.

---

### 3. Examiner les décisions mises à jour automatiquement

Naviguez directement vers les feuilles d'analyse.

Le classeur actualise immédiatement :

- les engagements de précommande en cours
- l'analyse des retours par cohorte
- la demande corrigée
- les recommandations d'achat
- la répartition par pays
- l'état de rapprochement

Aucun calcul manuel n'est nécessaire.

---

### 4. Actualiser chaque semaine

Chaque cycle de planification remplace simplement les tables d'entrée brutes.

Tout ce qui se trouve en aval se met à jour automatiquement.

Il n'y a ni reconstruction du classeur, ni copie de formules, ni maintenance structurelle.

**Définissez quelques paramètres opérationnels. Importez vos données existantes. Examinez les recommandations. Actualisez dès que de nouvelles données métier sont disponibles.**

---

## Pourquoi j'ai conçu cet outil

De nombreux problèmes de planification des stocks ne sont pas causés par de mauvais algorithmes de prévision.

Ils sont causés par de mauvais signaux de demande.

Pour les marques exploitant plusieurs boutiques Shopify, en particulier les entreprises de mode fortement axées sur les précommandes et affichant des taux de retour élevés, les ventes déclarées contiennent souvent des signaux qui ne devraient jamais devenir de la demande d'achat.

Une précommande est enregistrée comme une vente avant que le stock n'existe.

Un article retourné peut ne pas réintégrer le stock avant plusieurs semaines.

Les planificateurs de stocks reçoivent fréquemment des ventes historiques sans comprendre ni l'une ni l'autre de ces conditions.

Le résultat est prévisible :

- acheter deux fois pour la même demande,
- surestimer les besoins futurs en stock,
- accumuler du stock inutile,
- augmenter le fonds de roulement sans augmenter les revenus.

---

J'ai conçu ce projet parce que j'ai observé à maintes reprises des analystes passer des heures à nettoyer les données avant même de pouvoir commencer à prendre des décisions d'achat.

Plutôt que de créer un tableau de bord supplémentaire, j'ai voulu encapsuler le processus de raisonnement lui-même dans un classeur réutilisable.

Par exemple :

**Avant**

Un SKU vend **500 unités** lors d'un lancement.

La planification traditionnelle suppose que la demande est égale à 500.

Les recommandations d'achat sont générées à partir de ce chiffre.

---

**Après**

Le classeur découvre :

- 120 unités sont encore des précommandes non exécutées.
- Les retours attendus s'élèvent à 48 unités.
- La demande corrigée devient **332 unités**.

La conversation sur les achats change immédiatement.

Au lieu de discuter de la rapidité avec laquelle recommander 500 unités, les équipes opérationnelles se demandent si 332 unités suffisent après prise en compte du délai d'approvisionnement et du stock de sécurité.

C'est une décision fondamentalement différente—non pas parce que les formules ont changé, mais parce que le signal de demande est devenu fiable.

---

## Problèmes courants de planification des stocks résolus par cet outil

| Problème | Sans cet outil | Avec cet outil |
|----------|-------------------|----------------|
| Les précommandes gonflent la demande | Les achats dupliquent un stock déjà engagé | Les engagements en cours sont isolés avant la prévision |
| Les retours faussent les ventes historiques | Les prévisions supposent que toutes les ventes deviennent une demande permanente | La modélisation des retours par cohorte estime le stock récupérable |
| Plusieurs pays se disputent le stock | La répartition manuelle crée des niveaux de stock incohérents | La répartition suit des ratios de contribution des marchés configurables |
| Les décisions d'achat reposent sur des systèmes déconnectés | Les analystes comparent Shopify, Inventory Planner et l'ERP manuellement | Le rapprochement automatisé signale les quantités divergentes |
| La planification hebdomadaire exige de reconstruire les feuilles | La copie de formules introduit des erreurs cachées | Les données brutes sont actualisées tandis que les calculs restent inchangés |
| Les problèmes de stock sont découverts trop tard | Les erreurs d'achat apparaissent après la création du bon de commande | Le rapprochement expose les écarts avant l'émission des commandes |

---

## À qui s'adresse cet outil

Ce projet est conçu pour les organisations qui pilotent des décisions de stock sur plusieurs marchés, où les signaux de demande sont influencés par les précommandes, les retours et l'exécution internationale.

Les utilisateurs typiques sont :

- les marques de mode DTC
- les équipes opérationnelles Shopify
- les planificateurs de stocks
- les analystes de la chaîne logistique
- les équipes de planification des assortiments
- les responsables des opérations e-commerce

Il est particulièrement précieux lorsque les décisions d'achat dépendent de la compréhension de la différence entre les **ventes déclarées** et la **demande réelle en stock**.

Il n'est **pas** destiné à remplacer les plateformes ERP, les systèmes de gestion d'entrepôt ou les logiciels de stock d'entreprise.

Au lieu de cela, il fournit une couche analytique légère entre les systèmes opérationnels et les décisions d'achat.

Aucune expertise en tableur n'est requise. Ouvrez la version navigateur ou le classeur Excel, importez vos données opérationnelles et commencez immédiatement à examiner les recommandations d'achat.

---

## À propos

Je conçois des classeurs analytiques légers pour des situations métier où il y a tout simplement trop de pièces en mouvement pour les raisonner mentalement.

Plutôt que de remplacer les logiciels d'entreprise, ces outils organisent les informations nécessaires pour prendre la prochaine décision opérationnelle avec confiance.

La **Console de gouvernance des stocks DTC transfrontalière** est un exemple de cette approche : transformer des données opérationnelles fragmentées en un cadre d'aide à la décision reproductible, actualisable dès que de nouvelles informations sont disponibles.

## Détails techniques

<details>
<summary><strong>Pour les réviseurs techniques, les praticiens d'Excel et les collaborateurs</strong></summary>

---

## Architecture du classeur

Le classeur suit une architecture stricte de type **entrée → nettoyage → décision → validation → sortie**. Chaque feuille a une responsabilité unique, ce qui rend le processus analytique transparent et auditable.

| Couche | Feuille | Objectif | Consommateur de sortie |
|--------|-----------|---------|-----------------|
| Configuration | Config | Règles métier, délai d'approvisionnement, ratios de répartition, fenêtre de retour | Toutes les feuilles de calcul |
| Entrée brute | Raw_Orders | Exportations de commandes Shopify | Moteur de demande |
| Entrée brute | Raw_Returns | Exportations de retours Shopify | Modèle de retours |
| Nettoyage | Preorder_Liability | Engagements de précommande en cours | Demande corrigée, planificateur d'achats |
| Nettoyage | Cohort_Return_Model | Comportement des retours par cohorte | Demande corrigée |
| Décision | Corrected_Demand | Demande d'achat réelle | Inventory Planner |
| Décision | PO_Planner | Recommandations d'achat | Équipe achats |
| Décision | Location_Allocator | Répartition par pays | Entrepôts et logistique |
| Validation | Reconciliation | Vérification inter-systèmes | Opérations |
| Présentation | Executive_Dashboard | Indicateurs de gestion | Direction |

### Flux de données global

```text
Shopify Orders
                     \
                      \
                       --> Raw_Orders ------------------\
                                                        \
                                                         \
Inventory Planner Export --> Current Inventory -----------> PO Planner
                                                          /
                                                         /
Shopify Returns --> Raw_Returns --> Cohort Return Model-/

                     Config Parameters
                             │
                             ▼
                 Preorder Liability Engine
                             │
                             ▼
                 Corrected Demand Engine
                             │
                             ▼
                Purchase Recommendation
                             │
                             ▼
                  Country Allocation
                             │
                             ▼
                    Reconciliation
                             │
                             ▼
                 Executive Dashboard
```

Contrairement aux tableurs traditionnels où les calculs sont dispersés sur plusieurs feuilles, ce classeur sépare les responsabilités opérationnelles en couches analytiques indépendantes.

Cette séparation permet de remonter chaque recommandation d'achat jusqu'aux données opérationnelles qui l'ont produite.

---

## Trois pièges analytiques qui trompent même les planificateurs de stocks expérimentés

---

## Piège 1 — Traiter les précommandes comme une demande finalisée

### Décision

L'équipe achats augmente la production après avoir observé des ventes exceptionnellement fortes.

### Hypothèse cachée

On suppose que les ventes déclarées représentent la demande client exécutée.

En réalité, une grande partie de ces ventes sont encore des précommandes en cours.

### Pourquoi cela change la recommandation

| Indicateur | Vue traditionnelle | Vue corrigée |
|---------|-----------------|----------------|
| Ventes | 1 000 | 1 000 |
| Précommandes en cours | ignorées | 280 |
| Demande d'achat | 1 000 | 720 |

Sans isoler les engagements en cours, les planificateurs de stocks achètent des produits que les clients se sont déjà engagés à acheter.

Cela crée des achats en double.

### Pourquoi ce raisonnement est erroné

Les ventes décrivent l'activité commerciale.

L'achat devrait répondre aux obligations de stock physiques.

Ce ne sont pas toujours la même chose.

En particulier pour les lancements de mode, le financement participatif et les longs délais de fabrication.

### Approche corrigée

Les précommandes en cours sont isolées avant que la demande n'entre dans le modèle d'achat.

Seule la demande exécutée contribue aux besoins d'achat futurs.

### Résultat de la décision

Au lieu d'augmenter la production de 1 000 unités,

les équipes opérationnelles achètent du stock pour environ 720 unités,

ce qui réduit l'investissement en stock inutile tout en protégeant les engagements clients.

<details>
<summary>Logique de la formule</summary>

```excel
Outstanding Liability

=
Total Preorder Sold
-
Fulfilled Preorders
```

Implémenté à l'aide de formules de tableau dynamiques et de SUMIFS.

</details>

---

## Piège 2 — Mesurer les retours par mois civil

### Décision

La direction conclut que les taux de retour ont baissé parce que les retours de ce mois semblent plus faibles.

### Hypothèse cachée

On suppose que les retours survenus pendant un mois civil appartiennent aux ventes réalisées durant ce même mois.

Cette hypothèse n'est presque jamais vraie.

Les retours sont liés aux cohortes d'achat plutôt qu'aux périodes de reporting.

### Pourquoi cela change la recommandation

Exemple :

| Mois | Ventes | Retours du calendrier |
|--------|-------|-----------------|
| Janvier | 8 000 | 220 |
| Février | 6 500 | 640 |

Le reporting traditionnel suggère que les produits de février performent moins bien.

Cependant, la plupart des retours de février appartiennent en réalité aux achats de janvier.

### Pourquoi ce raisonnement est erroné

Le comportement des clients suit l'âge de la commande.

Les rapports suivent les dates du calendrier.

Ces deux chronologies coïncident rarement.

### Approche corrigée

Les commandes sont regroupées par cohorte d'achat.

Les retours sont mesurés :

- sous 14 jours
- sous 30 jours
- sous 45 jours

Le profil de retour qui en résulte reflète le comportement réel des clients au lieu d'artefacts de reporting.

### Résultat de la décision

Au lieu de réduire les achats de février,

l'entreprise découvre que les produits de janvier ont connu des retours tardifs,

tandis que la demande de février reste saine.

<details>
<summary>Logique de la formule</summary>

```excel
Unique Cohort Months

=SORT(
UNIQUE(
TEXT(Order_Date,"yyyy-mm")
))
```

Combiné avec MAP(), LET() et SUMIFS() pour calculer dynamiquement les fenêtres de retour.

</details>

---

## Piège 3 — Acheter à partir des ventes brutes plutôt qu'à partir de la demande corrigée

### Décision

Inventory Planner reçoit des ventes historiques exportées.

Les prévisions semblent raisonnables.

L'achat crée pourtant un stock excédentaire.

### Hypothèse cachée

On suppose que les ventes historiques représentent déjà une demande propre.

C'est rarement le cas.

Les ventes historiques incluent souvent :

- des précommandes en cours
- des retours attendus
- des pics de lancement temporaires

### Avant

```text
Historical Sales

980
```

Inventory Planner prévoit à partir de 980.

### Après nettoyage

```text
Historical Sales          980

Outstanding Liability    -170

Expected Returns          -62

Corrected Demand          748
```

### Pourquoi ce raisonnement est erroné

Les algorithmes de prévision amplifient la qualité des entrées.

Ils ne peuvent pas réparer de mauvais signaux historiques.

Des données erronées en entrée produisent toujours des résultats erronés en apparence fiables.

### Approche corrigée

La demande est corrigée avant d'entrer dans le logiciel de prévision.

Inventory Planner reçoit la demande d'achat plutôt que l'activité commerciale.

### Résultat de la décision

Les recommandations d'achat deviennent nettement plus stables.

Le fonds de roulement diminue tout en maintenant les niveaux de service client.

<details>
<summary>Logique de la formule</summary>

```excel
Corrected Demand

=
Raw Sales
-
Outstanding Liability
-
Expected Returns
```

Implémenté à l'aide de LET(), XLOOKUP(), SUMIFS() et de tableaux dynamiques.

</details>

---

## Scénario d'exemple

Une marque de mode basée au Royaume-Uni lance une nouvelle veste sur quatre boutiques Shopify desservant le Royaume-Uni, les États-Unis, l'UE et l'Australie.

En deux semaines, Shopify déclare **2 450 unités vendues**, ce qui suggère un lancement très réussi. Sur la seule base des ventes brutes, l'équipe achats envisage de passer une commande de réapprovisionnement urgente.

Le classeur raconte une histoire différente.

Tout d'abord, la feuille **Preorder_Liability** identifie **540 unités** vendues mais pas encore exécutées. Celles-ci représentent des engagements clients existants plutôt qu'une demande de marché supplémentaire.

Ensuite, le **Cohort_Return_Model** évalue le comportement historique des retours pour des produits comparables. Les lancements précédents montrent un taux de retour ultime de **11,8 %**, ce qui indique qu'environ **289 unités** devraient revenir en stock après la livraison.

Le moteur **Corrected_Demand** recalcule ensuite le signal d'achat :

| Poste | Quantité |
|------|---------:|
| Ventes déclarées | 2 450 |
| Précommandes en cours | -540 |
| Retours attendus | -289 |
| Demande corrigée | **1 621** |

Plutôt que d'acheter en fonction du chiffre de ventes global, **PO_Planner** utilise la demande corrigée ainsi que le délai d'approvisionnement, le stock actuel et les paramètres de sécurité pour recommander une quantité de réapprovisionnement nettement plus faible.

La recommandation est automatiquement répartie entre les entrepôts du Royaume-Uni, des États-Unis, de l'UE et d'Australie selon les ratios de répartition configurés.

Enfin, la feuille **Reconciliation** compare les engagements Shopify aux données de synchronisation d'Inventory Planner. Si les obligations en cours diffèrent entre les systèmes, le classeur déclenche un avertissement **INVESTIGATE** avant l'émission des bons de commande.

Le résultat est une décision d'achat appuyée sur des preuves opérationnelles rapprochées plutôt que sur des totaux de ventes brutes, ce qui réduit le stock excédentaire tout en maintenant les engagements d'exécution envers les clients.

---

### Référence des formules

<details>
<summary>Config</summary>

| Formule / Logique | Objectif | Remarques |
|-----------------|---------|------|
| Configuration manuelle | Définit les paramètres opérationnels | Mis à jour uniquement lors d'un changement des règles métier |
| Ratio de répartition des marchés | Répartition des stocks par pays | Utilisé par Location_Allocator |
| Délai d'approvisionnement | Planification des achats | Inclus dans le calcul du stock cible |
| Fenêtre de retour | Analyse par cohorte | Contrôle le calendrier des retours attendus |
| Facteur de sécurité des précommandes | Tampon d'achat | Ajustable par marché |

</details>

---

<details>
<summary>Preorder_Liability</summary>

### Générer la liste des SKU uniques

```excel
=SORT(
UNIQUE(
Raw_Orders[SKU]
))
```

**Objectif**

Crée une liste maîtresse de SKU dynamique directement à partir de l'historique des commandes importé.

---

### Engagements de précommande en cours

```excel
=LET(

SKU_List,A2#,

Preorder_Sold,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder"
),

Preorder_Fulfilled,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder",
Raw_Orders[Fulfillment_Status],"Fulfilled"
),

Preorder_Sold-
Preorder_Fulfilled

)
```

**Objectif**

Calcule les obligations de stock déjà vendues mais pas encore physiquement livrées.

Ces quantités sont volontairement exclues de la demande d'achat future.

---

</details>

---

<details>
<summary>Cohort_Return_Model</summary>

### Générer les mois de cohorte

```excel
=SORT(
UNIQUE(
TEXT(
Raw_Orders[Order_Date],
"yyyy-mm"
)
))
```

---

### Calcul des retours par cohorte

Implémenté avec

- LET()
- MAP()
- SUMIFS()

Le calcul mesure les retours par rapport à la date de commande d'origine plutôt qu'aux périodes de reporting calendaires.

Les fenêtres de retour comprennent :

- 14 jours
- 30 jours
- 45 jours

Cela produit une estimation stable du comportement de retour ultime.

---

### Taux de retour ultime

```text
Ultimate Return Rate

=

Total Returned Quantity

/

Original Cohort Sales
```

Le classeur exploite le comportement par cohorte plutôt que les pourcentages de retour mensuels, car les décisions d'achat dépendent du comportement des clients et non des périodes de reporting.

</details>

---

<details>
<summary>Corrected_Demand</summary>

### Signal de demande corrigé

```excel
=LET(

RawSales,

SUMIFS(...),

Outstanding,

XLOOKUP(...),

ExpectedReturns,

RawSales*
AverageReturnRate,

ROUND(

RawSales
-
Outstanding
-
ExpectedReturns,

0)

)
```

### Objectif

Transforme l'activité commerciale en demande d'achat.

Au lieu de prévoir directement à partir des ventes historiques, le classeur supprime :

- les précommandes en cours
- le stock dont le retour est attendu via les retours clients

Le signal résultant est adapté à Inventory Planner ou à un logiciel de prévision similaire.

</details>

---

<details>
<summary>PO_Planner</summary>

### Besoin d'achat net

```text
Net Requirement

=

Target Inventory

-

Current Stock

+

Outstanding Liability
```

---

### Quantité d'achat recommandée

```excel
=IF(

NetRequired<=0,

0,

MROUND(

NetRequired,

MOQ

)

)
```

### Objectif

Recommande automatiquement des quantités d'achat tout en respectant les quantités minimales de commande des fournisseurs.

Plutôt que d'exiger un arrondi manuel, les recommandations d'achat sont immédiatement propres à l'émission de bons de commande.

</details>

---

<details>
<summary>Location_Allocator</summary>

### Répartition par pays

```excel
=ROUND(

Total_PO

*

Allocation_Ratio,

0
)
```

Chaque entrepôt de destination reçoit du stock selon des ratios de contribution des marchés configurables.

Le modèle de répartition peut facilement être étendu à des pays supplémentaires sans modifier les calculs en aval.

</details>

---

<details>
<summary>Reconciliation</summary>

### Vérification de synchronisation

```excel
=IF(

Gap=0,

"PASS",

"INVESTIGATE"

)
```

où

```text
Gap

=

Shopify Unfulfilled

-

Inventory Planner Liability
```

Objectif :

Signale immédiatement les problèmes de synchronisation avant que les décisions d'achat ne s'appuient sur des données incohérentes.

</details>

---

## Règles de validation

| Champ | Règle de validation | Comportement en cas d'erreur |
|------|-----------------|----------------|
| Market | Doit exister dans la table Config | La recherche renvoie une répartition par défaut ou un avertissement de validation |
| SKU | Ne peut pas être vide | Ligne exclue des calculs |
| Order_ID | Doit être unique | Avertissement de transaction en double |
| Return_ID | Doit être unique | Avertissement de retour en double |
| Order Date | Date valide requise | Enregistrement ignoré jusqu'à correction |
| Return Date | Ne peut pas précéder Order Date | Marqueur de validation généré |
| Quantity | Doit être supérieure à zéro | Ligne exclue |
| Return Quantity | Ne peut pas dépasser la quantité d'origine | Avertissement de validation |
| Sales Type | Uniquement Normal ou Preorder | Catégorie invalide signalée |
| Fulfillment Status | Fulfilled / Unfulfilled | Valeurs invalides exclues |
| Allocation Ratio | Le total doit être égal à 100 % | Avertissement de répartition par pays |
| Lead Time | Entier non négatif | Le calcul d'achat est interrompu |
| Return Window | Entier positif | Avertissement sur le calcul de cohorte |
| MOQ | Supérieur à zéro | Recommandation d'achat désactivée |
| Current Inventory | Ne peut pas être négatif | Avertissement de stock |
| Outstanding Liability | Ne peut pas dépasser les ventes de précommande | Alerte de rapprochement |
| Recommended Purchase Quantity | Arrondie au MOQ | Ajustée automatiquement |
| Synchronization Gap | Doit être égal à zéro | Le statut INVESTIGATE est affiché |

</details>

---

## Autres outils de cette série

Ces classeurs suivent la même philosophie de conception : des systèmes d'aide à la décision légers, conçus pour des problèmes opérationnels récurrents plutôt que comme des remplaçants de logiciels d'entreprise.

- **Prévision des stocks et planification du réapprovisionnement** — Prévision de la demande, calcul du point de commande et analyse du risque de stock.
- **Construction Estimating System** — Estimation d'assemblages, bibliothèques de coûts, préparation des offres et budgétisation de projet.
- **Marketing Budget Allocation Simulator** — Planification par scénarios pour les investissements marketing multicanaux.
- **Multi-Currency Trade Finance Dashboard** — Reporting financier transfrontalier et analyse de rentabilité.
- **Coffee Shop Operations Audit Toolkit** — Évaluation de la performance des points de vente et analyse de la conformité opérationnelle.
- **Project Management & Progress Billing Console** — Suivi des jalons, facturation et contrôle budgétaire.

D'autres classeurs analytiques seront publiés via le dépôt GitHub et notre [Site web](https://www.theseusworkshop.com/).

---

## Licence

Ce projet est sous licence **Apache License 2.0**.

Vous êtes libre de :

- utiliser le classeur à des fins personnelles ou commerciales.
- modifier le cadre analytique pour l'adapter aux exigences opérationnelles.
- distribuer des versions modifiées conformément à la Apache License 2.0.

Consultez le fichier **LICENSE** pour le texte intégral de la licence.

---

## Notes finales

Ce classeur est délibérément positionné comme une **couche d'aide à la décision**, et non comme un remplaçant des plateformes ERP, WMS ou de planification d'entreprise.

Son objectif est simple :

- capturer les données opérationnelles des systèmes existants,
- supprimer les distorsions analytiques avant la planification,
- générer des recommandations d'achat qui reflètent les obligations de stock réelles,
- fournir des calculs transparents qui peuvent être inspectés, reproduits et audités.

Au lieu d'ajouter un tableau de bord de plus, le classeur industrialise une méthodologie de planification des stocks reproductible, actualisable en quelques minutes et compréhensible tant par les utilisateurs opérationnels que par les réviseurs techniques.
