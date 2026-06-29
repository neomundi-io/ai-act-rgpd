🌐 **Langues :** [Français](README.md) · [English](README_EN.md)

---

# NeoMundi ControlTower

## Preuve en exploitation, surveillance continue et traçabilité pour la gouvernance de l’IA

NeoMundi ControlTower est une couche de diagnostic, de surveillance continue et de traçabilité pour les réponses générées par des systèmes d’IA.

Elle aide les organisations à observer les signaux comportementaux en exploitation, détecter des dérives ou changements de régime mesurables, documenter des indicateurs de risque, appliquer des mécanismes de gouvernance configurables et maintenir des preuves techniques des contrôles disponibles et mobilisés.

ControlTower est conçu selon une approche *privacy-first*. Il peut être intégré par un simple appel API, sans modification de l’infrastructure IA sous-jacente, et peut être déployé dans des environnements souverains selon le modèle de déploiement retenu.

Ce document présente :

1. ce que ControlTower couvre techniquement aujourd’hui ;
2. comment ces capacités peuvent contribuer au processus de conformité d’une organisation au regard de l’AI Act européen et du RGPD ;
3. ce qui reste en dehors du périmètre de NeoMundi et relève de la responsabilité de chaque organisation.

> **Important :** NeoMundi ne détermine pas si un système d’IA est juridiquement conforme.
> Il fournit une couche de preuve en exploitation qui aide les organisations à observer les dérives comportementales, documenter les signaux de risque, déclencher une revue humaine adaptée et démontrer que des contrôles opérationnels existaient lorsqu’ils étaient nécessaires.

---

# 1. Ce que ControlTower couvre réellement

## 1.1. Traçabilité opérationnelle des réponses IA observées

ControlTower associe les événements observés liés aux réponses d’IA à des artefacts techniques et opérationnels pouvant inclure :

* un identifiant d’observation ;
* des métriques calculées ;
* des signaux de risque mesurés ;
* un statut de gouvernance ou de contrôle configurable ;
* des horodatages d’observation ;
* un historique de mesure configurable ;
* des artefacts de traçabilité adaptés au mode de déploiement sélectionné ;
* des éléments de justification associés aux règles ou actions configurées.

Ces artefacts permettent de relier un comportement observé à des signaux techniques et à un contexte de contrôle disponibles au moment de l’observation.

### Capacité couverte

**Traçabilité technique et opérationnelle du comportement observé des réponses IA et des signaux de risque associés.**

---

## 1.2. Surveillance continue du comportement des réponses IA

ControlTower observe en continu des signaux associés au comportement des systèmes d’IA pendant leur fonctionnement.

Selon les modules activés et la configuration retenue, ces signaux peuvent inclure :

* la stabilité ;
* la cohérence ;
* la variation sémantique ;
* la dérive comportementale ;
* des indicateurs de risque d’hallucination ;
* des indicateurs de risque factuel ;
* des signaux liés à la validité factuelle lorsque le module concerné est activé ;
* des indicateurs de latence, d’exécution ou d’exploitation ;
* des signaux de risque configurables associés aux réponses générées.

L’objectif n’est pas d’affirmer qu’un signal établit, à lui seul, la vérité ou l’erreur d’une réponse.

L’objectif est de rendre observable le moment où le comportement mesuré d’un système évolue, devient fragile, dépasse un seuil défini ou nécessite une revue complémentaire.

### Capacité couverte

**Surveillance continue du comportement des réponses IA, de leur variabilité et de signaux de risque opérationnels mesurables.**

---

## 1.3. Détection des dérives comportementales et des changements de régime silencieux

ControlTower peut aider à identifier des évolutions mesurables du comportement d’un système d’IA dans le temps.

Un changement comportemental peut apparaître même lorsque :

* aucune mise à jour publique du fournisseur n’a été annoncée ;
* aucun incident visible en production n’a encore été signalé ;
* un benchmark ponctuel demeure globalement rassurant ;
* des instantanés de qualité conventionnels ne révèlent pas ce changement.

Ces observations peuvent notamment concerner des évolutions de signaux de risque factuel, de variation sémantique, de stabilité ou d’autres indicateurs suivis.

ControlTower n’attribue pas la cause d’un changement comportemental détecté, sauf lorsqu’une investigation indépendante permet de l’établir.

Un signal détecté constitue une observation opérationnelle. Il ne constitue pas, à lui seul, la preuve d’un changement de fournisseur, d’un défaut système, d’un manquement juridique ou d’une cause racine.

### Capacité couverte

**Détection et traçabilité de dérives comportementales mesurables et de changements de régime silencieux en exploitation.**

---

## 1.4. Mécanismes configurables de gouvernance et de contrôle

ControlTower peut prendre en charge des mécanismes de gouvernance configurables, appliqués en temps réel ou quasi temps réel selon l’intégration choisie.

Ces mécanismes peuvent inclure :

* des seuils de risque ;
* des alertes ;
* des parcours d’escalade ;
* l’orientation vers une revue humaine ;
* un traitement différencié des réponses à risque plus élevé ;
* des mécanismes configurables de blocage ou de mise en attente, lorsque l’intégration retenue le permet ;
* des journaux d’observation et de décision ;
* l’audit de l’application des règles et de l’historique de mesure.

ControlTower ne transforme pas silencieusement un signal observé en action autorisée.

Un signal de mesure peut justifier une information, une revue ou une escalade, mais l’autorité d’agir demeure définie par les règles de gouvernance de l’organisation, les rôles responsables et l’intégration retenue.

### Capacité couverte

**Surveillance continue et mécanismes configurables de contrôle du risque lié aux réponses IA.**

---

## 1.5. Support à la supervision humaine

ControlTower peut soutenir la supervision humaine en rendant les signaux pertinents en exploitation visibles et exploitables.

Selon la configuration, la plateforme peut aider les organisations à :

* définir des seuils nécessitant une revue ;
* notifier les équipes responsables ;
* escalader les observations présentant un risque plus élevé ;
* orienter les événements vers un relecteur désigné ;
* conserver la preuve de l’observation et de son contexte de contrôle ;
* distinguer un signal observé d’une décision aval autorisée.

La plateforme fournit un support technique à la supervision humaine. Elle ne remplace ni le jugement humain, ni la responsabilité organisationnelle, ni la responsabilité juridique.

### Capacité couverte

**Support technique à une supervision humaine, une revue et une escalade fondées sur le risque.**

---

## 1.6. Auditabilité et preuve en exploitation

ControlTower produit des éléments techniques mesurables et vérifiables pouvant inclure :

* des métriques ;
* des scores ;
* des signaux de risque ;
* des identifiants d’observation ;
* un historique configurable ;
* des artefacts de mesure ;
* des artefacts d’application des règles ;
* des éléments de justification ;
* des preuves techniques associées aux événements observés.

Ces éléments peuvent être utilisés pour soutenir un audit interne, une analyse d’incident, une revue opérationnelle, un reporting de gouvernance ou des démarches d’assurance par des tiers.

### Capacité couverte

**Auditabilité du comportement observé des réponses IA, des signaux mesurés et des mécanismes de contrôle configurés.**

---

## 1.7. Gouvernance opérationnelle fondée sur des preuves

ControlTower ne repose pas uniquement sur une promesse déclarative de fiabilité d’un système d’IA.

Il fournit des signaux mesurés, traçables et configurables qui peuvent aider les organisations à rendre leurs processus de gouvernance plus explicites.

Par exemple, une organisation peut utiliser ControlTower pour documenter que :

* une observation a été détectée ;
* un signal de risque a franchi un seuil configuré ;
* un rôle responsable a été notifié ;
* une revue humaine a été demandée ;
* un mécanisme de contrôle défini était disponible ou a été appliqué ;
* la décision aval finale est restée soumise à l’autorité de l’organisation.

### Capacité couverte

**Gouvernance opérationnelle soutenue par des preuves mesurées et traçables en exploitation.**

---

# 2. Architecture privacy-first

ControlTower est conçu selon des principes de protection des données dès la conception.

Selon le mode de déploiement et la configuration sélectionnés, son architecture vise à minimiser l’exposition au contenu et à limiter le traitement aux données nécessaires à la mesure, à la surveillance et aux mécanismes de gouvernance configurés.

Les principes structurants incluent :

* zéro rétention de contenu ;
* zéro journalisation de contenu ;
* zéro stockage de contenu ;
* minimisation des données ;
* traçabilité configurable ;
* flexibilité de déploiement, y compris des modèles de déploiement souverains lorsque disponibles.

Les contenus des prompts et des réponses ne sont ni conservés, ni indexés, ni réutilisés, ni stockés par NeoMundi.

Des artefacts techniques minimaux de mesure et de traçabilité peuvent rester disponibles selon le mode sélectionné, la configuration et le modèle de déploiement retenu.

---

## 2.1. Mode OBS

En mode OBS, NeoMundi reçoit uniquement les éléments techniques nécessaires à l’observation.

Cela peut inclure :

* des métriques normalisées ;
* des artefacts techniques d’observation ;
* des identifiants ou références pseudonymes requis pour la traçabilité configurée ;
* des signaux opérationnels agrégés ou non liés au contenu.

NeoMundi ne reçoit pas :

* les prompts bruts ;
* les réponses brutes ;
* le contenu sémantique stocké des échanges ;
* du contenu client destiné à être réutilisé ou indexé.

### Capacité couverte

**Observation du risque et traçabilité technique sans transmission ni rétention du contenu des prompts et des réponses.**

---

## 2.2. Mode GOV

En mode GOV, des données peuvent transiter en temps réel uniquement à des fins de mesure et d’application de règles de gouvernance configurées.

Le contenu :

* n’est pas retenu ;
* n’est pas indexé ;
* n’est pas réutilisé ;
* n’est pas stocké.

Le fonctionnement précis du mode GOV dépend de l’intégration retenue, du modèle de déploiement et de la configuration de l’organisation.

### Capacité couverte

**Mesure en temps réel et mécanismes de gouvernance configurables sans rétention de contenu.**

---

## 2.3. Options de déploiement souverain

ControlTower peut être déployé selon un modèle d’infrastructure souveraine ou contrôlée, en fonction de l’architecture de déploiement retenue.

Cela peut répondre aux besoins d’organisations nécessitant :

* des environnements d’hébergement contrôlés ;
* des contraintes de localisation des données ;
* une souveraineté des infrastructures ;
* une intégration avec des environnements cloud de confiance ou sur site ;
* une réduction de l’exposition des données opérationnelles liées à l’IA.

### Capacité couverte

**Flexibilité de déploiement pour les organisations ayant des exigences de souveraineté, de sécurité ou de contrôle de l’infrastructure.**

---

# 3. Comment ControlTower peut contribuer à un processus de conformité à l’AI Act européen

ControlTower ne remplace ni l’analyse juridique, ni l’évaluation de conformité, ni la gouvernance organisationnelle, ni une certification réglementaire.

Il fournit toutefois des capacités techniques et des preuves en exploitation qui peuvent contribuer à plusieurs domaines opérationnels pertinents dans le cadre d’un processus de conformité à l’AI Act européen.

L’applicabilité de ces domaines dépend du système d’IA concerné, de sa finalité prévue, du rôle de l’organisation, de la classification de risque du système et du cas d’usage spécifique.

| Domaine opérationnel                                | Contribution de ControlTower                                                                                 | Niveau de couverture                           |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | ---------------------------------------------- |
| Surveillance pendant l’exploitation                 | Observation continue du comportement des réponses IA, de leur variabilité et de signaux de risque configurés | Techniquement pris en charge                   |
| Support à la gestion des risques                    | Scores mesurés, signaux de risque, seuils, alertes et mécanismes d’escalade                                  | Techniquement pris en charge                   |
| Traçabilité opérationnelle                          | Identifiants d’observation, métriques, horodatages et artefacts de mesure configurables                      | Techniquement pris en charge                   |
| Support à la journalisation                         | Historique technique et artefacts de traçabilité configurables sans rétention de contenu                     | Pris en charge selon la configuration          |
| Support à la supervision humaine                    | Alertes, parcours d’escalade, orientation vers une revue humaine et visibilité des signaux mesurés           | Capacité technique fournie                     |
| Traitement de réponses à risque plus élevé          | Traitement différencié, revue, mise en attente ou blocage selon l’intégration                                | Capacité technique fournie selon l’intégration |
| Auditabilité                                        | Signaux mesurés, artefacts techniques et éléments de justification                                           | Techniquement pris en charge                   |
| Analyse et documentation d’incidents                | Preuves en exploitation pouvant soutenir l’analyse, l’investigation et la documentation d’événements         | Contribution opérationnelle directe            |
| Surveillance post-déploiement                       | Observation longitudinale du comportement, des dérives et des changements de régime mesurables               | Contribution opérationnelle directe            |
| Transparence des contrôles opérationnels            | Visibilité sur les signaux observés, les seuils configurés et le contexte de contrôle appliqué               | Contribution opérationnelle directe            |
| Classification juridique complète d’un système d’IA | Dépend de la finalité prévue, du cas d’usage, du rôle de l’organisation et de l’analyse juridique            | Hors périmètre                                 |
| Évaluation formelle de conformité                   | Nécessite le processus juridique, organisationnel et technique applicable                                    | Hors périmètre                                 |
| Certification réglementaire                         | Nécessite le processus de certification et d’évaluation approprié                                            | Hors périmètre                                 |

---

## 3.1. Preuve en exploitation pour la surveillance post-déploiement

Une contribution centrale de ControlTower réside dans la possibilité de créer un historique longitudinal du comportement observé d’un système d’IA pendant son fonctionnement.

Cela peut aider les organisations à identifier :

* une variation inattendue ;
* une hausse des signaux de risque factuel ;
* des changements de comportement sémantique ;
* une dégradation de la stabilité observée ;
* une évolution de la distribution des risques ;
* des changements de régime silencieux ;
* des schémas nécessitant une revue avant qu’ils ne deviennent visibles par les processus traditionnels de remontée d’incidents.

ControlTower ne remplace pas une investigation d’incident.

Il aide à établir qu’un signal opérationnel a été observé, mesuré et documenté à un instant donné, dans un contexte défini de mesure et de gouvernance.

---

## 3.2. La distinction entre mesure et autorisation

ControlTower est conçu autour d’une distinction de gouvernance essentielle :

> **Un signal de mesure en exploitation ne constitue pas, à lui seul, une autorisation d’agir.**

Un signal mesuré peut justifier :

* une information interne ;
* une investigation complémentaire ;
* une revue humaine ;
* une recommandation ;
* une escalade ;
* une réponse de sécurité configurée.

La possibilité de justifier une action aval dépend du modèle de gouvernance de l’organisation, de l’autorité responsable, du cas d’usage et des contrôles applicables.

Cette distinction contribue à éviter qu’un signal technique observé soit silencieusement traité comme une décision finale.

---

# 4. Comment ControlTower peut contribuer à un processus de conformité au RGPD

ControlTower est conçu pour soutenir des principes de traitement des données *privacy-first*.

Il ne remplace ni une analyse complète au regard du RGPD, ni le registre des activités de traitement, ni une analyse d’impact relative à la protection des données, ni la responsabilité juridique du responsable de traitement ou du sous-traitant.

Son architecture peut néanmoins apporter un support technique à plusieurs principes opérationnels liés au RGPD.

| Domaine lié au RGPD                                   | Contribution de ControlTower                                                                                 | Niveau de couverture                |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | ----------------------------------- |
| Minimisation des données                              | Transmission limitée aux données nécessaires selon le mode et la finalité technique retenus                  | Soutenu par l’architecture          |
| Protection des données dès la conception              | Les modes OBS et GOV visent à minimiser l’exposition au contenu et à éviter sa rétention                     | Soutenu par l’architecture          |
| Limitation de la conservation                         | Absence de rétention, de journalisation et de stockage des contenus de prompts et de réponses par NeoMundi   | Soutenu par l’architecture          |
| Support à l’accountability                            | Artefacts techniques pouvant aider à documenter les mécanismes de surveillance et de contrôle mis en œuvre   | Contribution opérationnelle directe |
| Traçabilité des contrôles                             | Signaux, métriques, identifiants et historique technique configurable                                        | Techniquement pris en charge        |
| Support à la documentation des traitements            | Éléments techniques pouvant contribuer à la documentation organisationnelle                                  | Contribution partielle              |
| Registre des activités de traitement                  | Document organisationnel et juridique maintenu par le responsable de traitement ou le sous-traitant concerné | Hors périmètre                      |
| Analyse d’impact relative à la protection des données | Évaluation juridique et organisationnelle réalisée lorsqu’elle est requise                                   | Hors périmètre                      |
| Détermination de la base légale                       | Dépend du contexte de traitement et de l’analyse juridique de l’organisation                                 | Hors périmètre                      |
| Gestion des droits des personnes concernées           | Nécessite des procédures et systèmes organisationnels allant au-delà de ControlTower                         | Hors périmètre                      |

---

# 5. Ce que ControlTower ne couvre pas

NeoMundi ne remplace pas les responsabilités juridiques, organisationnelles, de sécurité ou de gouvernance d’une organisation.

ControlTower ne fournit pas :

* la classification juridique complète d’un système d’IA au regard de l’AI Act européen ;
* un conseil juridique ;
* une analyse juridique d’un cas d’usage spécifique ;
* une confirmation automatique de conformité réglementaire ;
* la préparation du registre des activités de traitement d’une organisation ;
* la réalisation d’une analyse d’impact relative à la protection des données ;
* la politique interne IA d’une organisation ;
* la gouvernance RH ;
* la gestion de la conformité contractuelle ;
* la qualification complète des fournisseurs ;
* la cartographie du Shadow AI ;
* un audit global de cybersécurité ;
* une évaluation formelle de conformité ;
* une certification réglementaire ;
* l’attribution d’une cause racine à un changement comportemental observé ;
* la preuve qu’une réponse isolée est vraie, fausse, sûre ou conforme à partir d’un unique signal de mesure ;
* le remplacement du jugement humain ou de l’autorité organisationnelle responsable.

---

# 6. Positionnement résumé

**NeoMundi ControlTower est une couche de preuve en exploitation, de surveillance continue et de traçabilité pour les réponses générées par des systèmes d’IA.**

Il aide les organisations à :

* observer le comportement des réponses IA pendant leur fonctionnement ;
* détecter des dérives mesurables et des changements de régime silencieux ;
* documenter les signaux de risque et le contexte technique ;
* soutenir la supervision humaine et les mécanismes d’escalade ;
* appliquer des mécanismes de contrôle configurables ;
* maintenir des preuves opérationnelles auditables ;
* réduire l’exposition au contenu grâce à une architecture *privacy-first* ;
* contribuer, sans s’y substituer, aux processus de conformité à l’AI Act et au RGPD.

NeoMundi ne prétend pas déterminer si un système d’IA est juridiquement conforme.

Il fournit la couche de preuve opérationnelle qui aide les organisations à comprendre ce que leurs systèmes d’IA faisaient en production, quels signaux ont été observés, quels contrôles étaient disponibles et quelle réponse de gouvernance a été déclenchée.

---

# 7. Intégration

ControlTower peut être intégré :

* par un simple appel API ;
* sans nécessiter de modification de l’infrastructure IA sous-jacente ;
* en mode OBS ;
* en mode GOV ;
* selon des modèles de déploiement souverain en fonction de l’architecture retenue ;
* avec des paramètres configurables de surveillance, de seuils, d’alertes et de traçabilité.

Les capacités disponibles dépendent du modèle de déploiement sélectionné, de la profondeur d’intégration et de la configuration de l’organisation.

---

# 8. Avertissement

Ce document décrit les capacités techniques et la contribution opérationnelle visée par NeoMundi ControlTower.

Il ne constitue pas :

* un conseil juridique ;
* une certification réglementaire ;
* une évaluation formelle de conformité ;
* une garantie automatique de conformité ;
* une évaluation complète applicable à une organisation ou à un cas d’usage IA spécifique.

La conformité dépend de plusieurs facteurs, notamment :

* du système d’IA concerné ;
* de sa finalité prévue ;
* de sa classification de risque ;
* du contexte d’utilisation ;
* du rôle de l’organisation ;
* du cadre juridique applicable ;
* des mesures techniques et organisationnelles mises en œuvre ;
* des processus de gouvernance et de supervision humaine maintenus par l’organisation.
