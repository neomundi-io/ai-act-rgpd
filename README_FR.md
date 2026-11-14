<div align="center">

<sub><a href="README.md">English</a> · <b>Français</b></sub>

# NeoMundi — AI Act & RGPD

### De la mesure aux preuves techniques pour la gouvernance des IA.

**Mesurer les comportements, documenter les conditions d'observation et vérifier les éléments techniques pouvant contribuer à la gouvernance et aux démarches de conformité.**

**Measurement → Station → Evidence**

[![Measurement](https://img.shields.io/badge/Measurement-Mesurer-2563eb?style=flat-square)](https://github.com/neomundi-io/neomundi-runtime-measurement/blob/main/README_FR.md)
[![Station](https://img.shields.io/badge/Station-Observer-0f766e?style=flat-square)](https://github.com/neomundi-io/neomundi-station-public/blob/main/README.fr.md)
[![Evidence](https://img.shields.io/badge/Evidence-Verifier-D4A545?style=flat-square)](https://github.com/neomundi-io/neomundi-evidence-public/blob/main/README.fr.md)
[![Use cases](https://img.shields.io/badge/Cas_d_usage-Explorer-64748b?style=flat-square)](https://github.com/neomundi-io/neomundi-use-cases/blob/main/README_FR.md)

**[API](https://github.com/neomundi-io/neomundi-runtime-measurement/blob/main/QUICKSTART.md)** · **[Créer un compte](https://controltower.neomundi.io/welcome)**

</div>

---

> ### Qui exploite NeoMundi, et à quel stade
>
> NeoMundi est un **projet de recherche et développement** porté par
> **NeoMundi Recherche**, **association à but non lucratif régie par la loi
> du 1er juillet 1901**. Activité actuelle : recherche, développement,
> expérimentation et pilotes.
>
> **Les utilisateurs actuels sont des pilotes, non des clients commerciaux**,
> et aucune facturation n'est pratiquée à ce jour. Lisez chacune des
> capacités ci-dessous dans ce cadre : ce document met en regard des
> obligations et des capacités techniques, il ne constitue pas une offre
> commerciale.
>
> L'identité du responsable de traitement, les traitements effectués, les
> prestataires réellement utilisés et les règles de conservation sont
> publiés dans la documentation canonique
> [Protection des données & confidentialité](https://github.com/neomundi-io/neomundi-io-data-protection).
> **En cas de divergence, c'est ce dépôt qui prévaut** — celui-ci n'est pas
> une seconde source.

---

## Ce que NeoMundi apporte

Une organisation doit pouvoir expliquer ce que ses IA ont produit, dans quelles conditions, quels signaux ont été mesurés et quelles traces sont disponibles pour un contrôle. NeoMundi fournit un socle technique pour répondre à ces questions.

| Produit | Contribution opérationnelle | Documents utiles |
|---|---|---|
| **[Measurement](https://github.com/neomundi-io/neomundi-runtime-measurement)** | Mesures versionnées des réponses IA, statuts, couverture des évaluateurs et signaux de risque bornés. | [API et première mesure](https://github.com/neomundi-io/neomundi-runtime-measurement/blob/main/QUICKSTART.md) |
| **[Station](https://github.com/neomundi-io/neomundi-station-public)** | Campagnes d'observation, contexte d'exécution, journalisation, provenance et export des dossiers. | [Présentation](https://github.com/neomundi-io/neomundi-station-public/blob/main/README.fr.md) |
| **[Evidence](https://github.com/neomundi-io/neomundi-evidence-public)** | Vérification de l'intégrité d'archives, traçabilité des artefacts et contrôle d'attestations Ed25519. | [Mode d'emploi](https://github.com/neomundi-io/neomundi-evidence-public/blob/main/docs/EVIDENCE_USER_GUIDE.fr.md) · [Démonstration](https://github.com/neomundi-io/neomundi-evidence-public/blob/main/docs/EVIDENCE_TECHNICAL_DEMO.fr.md) |

**Ce qui est démontré :** une qualification expérimentale réelle Q-2 a traversé Measurement → Station → Evidence, avec attestation Ed25519 vérifiée. Verdict technique positif sur les contrôles exécutés ; **verdict global Q-2 PARTIAL**. Le dossier source demeure privé. Voir le [rapport de validation Evidence](https://github.com/neomundi-io/neomundi-evidence-public/blob/main/docs/EVIDENCE_VALIDATION_REPORT.fr.md).

## Où ces preuves peuvent être utiles

| Besoin de gouvernance | Contribution possible | Ce qui doit être établi pour chaque intégration |
|---|---|---|
| **Traçabilité et journalisation** | Identifiants, mesures, traces de campagne, empreintes et archives contrôlables | Captation, exhaustivité, export, conservation, droits d'accès |
| **Supervision humaine** | Signaux pour examen et escalade par les responsables désignés | Alertes et routage réellement configurés dans le système consommateur |
| **Suivi de qualité et de dérive** | Comparaison longitudinale de mesures compatibles dans des campagnes ou dispositifs instrumentés | Protocole, fréquence, couverture et seuils validés |
| **Analyse d'incident et audit** | Dossiers techniques traçables, résultats de vérification et attestations | Chaîne de conservation, données disponibles et périmètre de preuve |
| **Protection des données** | Possibilités de minimisation et d'exports sans contenu brut selon le chemin | Cartographie réelle des flux, évaluateurs, sous-traitants et rétention |

Cette matrice décrit une **contribution technique potentielle**, pas une certification de conformité ni la disponibilité universelle de tous les mécanismes. Le fonctionnement dépend de la voie API, de l'intégration et du déploiement. Les décisions d'autorisation, de blocage et de conformité restent sous la responsabilité de l'organisation.

## Calendrier AI Act — vérifié le 7 novembre 2026

Le [règlement (UE) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj?locale=fr), modifié notamment par le [règlement (UE) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj?locale=fr), prévoit une application échelonnée :

| Échéance | Principales dispositions |
|---|---|
| **2 février 2025** | Définitions, culture IA et interdictions initiales |
| **2 août 2025** | Règles relatives aux modèles d'IA à usage général |
| **2 août 2026** | Application de la majorité des autres règles, dont plusieurs obligations de transparence |
| **2 décembre 2026** | Nouvelles interdictions spécifiques et échéance transitoire de l'article 50(2) pour certains systèmes |
| **2 décembre 2027** | Obligations des systèmes à haut risque relevant de l'annexe III |
| **2 août 2028** | Obligations des systèmes à haut risque intégrés aux produits de l'annexe I |

**Sources primaires :** [calendrier Commission européenne](https://ai-act-service-desk.ec.europa.eu/en/ai-act/eu-ai-act-implementation-timeline) et [texte modificatif au Journal officiel](https://eur-lex.europa.eu/eli/reg/2026/1744/oj?locale=fr). Les obligations concrètes dépendent du rôle de l'organisation, de la finalité du système et des dispositions applicables.

## Documentation opérationnelle détaillée

Les sections suivantes conservent le référentiel AI Act/RGPD, les flux de données, les mécanismes possibles et leurs frontières. Les capacités décrites comme configurables sont à confirmer pour chaque parcours ; un score de mesure n'est jamais à lui seul une autorisation d'agir.

---

# 1. Ce que NeoMundi couvre réellement

## 1.1. Traçabilité opérationnelle des réponses IA observées

NeoMundi associe les événements observés liés aux réponses d’IA à des artefacts techniques et opérationnels pouvant inclure :

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

## 1.2. Suivi du comportement des réponses IA

NeoMundi observe en continu des signaux associés au comportement des systèmes d’IA pendant leur fonctionnement.

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

NeoMundi peut aider à identifier des évolutions mesurables du comportement d’un système d’IA dans le temps.

Un changement comportemental peut apparaître même lorsque :

* aucune mise à jour publique du fournisseur n’a été annoncée ;
* aucun incident visible en production n’a encore été signalé ;
* un benchmark ponctuel demeure globalement rassurant ;
* des instantanés de qualité conventionnels ne révèlent pas ce changement.

Ces observations peuvent notamment concerner des évolutions de signaux de risque factuel, de variation sémantique, de stabilité ou d’autres indicateurs suivis.

NeoMundi n’attribue pas la cause d’un changement comportemental détecté, sauf lorsqu’une investigation indépendante permet de l’établir.

Un signal détecté constitue une observation opérationnelle. Il ne constitue pas, à lui seul, la preuve d’un changement de fournisseur, d’un défaut système, d’un manquement juridique ou d’une cause racine.

### Capacité couverte

**Détection et traçabilité de dérives comportementales mesurables et de changements de régime silencieux en exploitation.**

---

## 1.4. Mécanismes configurables de gouvernance et de contrôle

NeoMundi peut prendre en charge des mécanismes de gouvernance configurables, appliqués en temps réel ou quasi temps réel selon l’intégration choisie.

Ces mécanismes peuvent inclure :

* des seuils de risque ;
* des alertes ;
* des parcours d’escalade ;
* l’orientation vers une revue humaine ;
* un traitement différencié des réponses à risque plus élevé ;
* des mécanismes configurables de blocage ou de mise en attente, lorsque l’intégration retenue le permet ;
* des journaux d’observation et de décision ;
* l’audit de l’application des règles et de l’historique de mesure.

NeoMundi ne transforme pas silencieusement un signal observé en action autorisée.

Un signal de mesure peut justifier une information, une revue ou une escalade, mais l’autorité d’agir demeure définie par les règles de gouvernance de l’organisation, les rôles responsables et l’intégration retenue.

### Capacité couverte

**Surveillance continue et mécanismes configurables de contrôle du risque lié aux réponses IA.**

---

## 1.5. Support à la supervision humaine

NeoMundi peut soutenir la supervision humaine en rendant les signaux pertinents en exploitation visibles et exploitables.

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

NeoMundi produit des éléments techniques mesurables et vérifiables pouvant inclure :

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

NeoMundi ne repose pas uniquement sur une promesse déclarative de fiabilité d’un système d’IA.

Il fournit des signaux mesurés, traçables et configurables qui peuvent aider les organisations à rendre leurs processus de gouvernance plus explicites.

Par exemple, une organisation peut utiliser NeoMundi pour documenter que :

* une observation a été détectée ;
* un signal de risque a franchi un seuil configuré ;
* un rôle responsable a été notifié ;
* une revue humaine a été demandée ;
* un mécanisme de contrôle défini était disponible ou a été appliqué ;
* la décision aval finale est restée soumise à l’autorité de l’organisation.

### Capacité couverte

**Gouvernance opérationnelle soutenue par des preuves mesurées et traçables en exploitation.**

---

# 2. Frontières de protection des données

NeoMundi est conçu pour soutenir la minimisation des données, mais NeoMundi comporte plusieurs flux distincts. Ce document ne formule aucune promesse générale de zéro transmission, zéro stockage ou zéro conservation.

Les frontières techniques actuellement examinées sont les suivantes :

* une requête de mesure REST peut inclure le prompt et la réponse lorsque l'appelant les fournit ;
* un parcours de génération SSE transmet des paramètres de génération et l'identifiant fournisseur configuré au service amont ;
* le texte soumis peut être traité par les évaluateurs et services activés ;
* Station documente un registre interne contenant les réponses et le contexte de mesure, tandis que son interface en lecture seule restitue des empreintes et longueurs plutôt que le texte brut ;
* l'export d'interopérabilité exclut par conception les prompts, réponses et identifiants bruts de fournisseur ou modèle.

Transmission, traitement, divulgation et conservation sont des questions distinctes. Les garanties de conservation et d'effacement doivent être établies pour chaque déploiement, service, évaluateur, journal, sauvegarde et stockage. Un export ou une interface de lecture sans texte brut ne prouve pas que le texte brut n'a jamais été traité ou stocké en amont.

[**Consulter la documentation canonique Protection des données et confidentialité →**](https://github.com/neomundi-io/neomundi-io-data-protection/blob/main/README_FR.md)

⚠ **Ces frontières ont été examinées le 7 novembre 2026, et l'une d'elles a
changé depuis.** Le **13 novembre 2026**, un garde de sortie a été déployé
et vérifié sur le service en fonctionnement : l'envoi de contenu à un
prestataire externe exige désormais une **autorisation nommée et explicite**,
et non plus la simple présence d'un identifiant. Présenté avec un
identifiant bien formé pour un prestataire hors liste blanche, le service
**refuse**. La liste blanche réellement servie, les prestataires concernés et
les transferts mesurés sont publiés dans le dépôt canonique lié ci-dessus —
non repris ici, afin qu'il y ait une source et non deux.

## 2.1. Parcours OBS

OBS est un libellé de couche de mesure, pas une garantie que la charge utile se limite aux métriques. Le parcours REST examiné peut recevoir llm_prompt et llm_response lorsque l'appelant les fournit. D'autres intégrations peuvent soumettre des objets d'exécution réduits, mais les mesures encore disponibles et leur provenance dépendent de la charge utile et du déploiement réels.

## 2.2. Parcours GOV et génération

Dans les parcours GOV ou de génération, le contenu et les paramètres fournisseur peuvent transiter par NeoMundi et les services amont configurés pour la mesure, la génération ou les contrôles activés. Les destinations, évaluateurs, mécanismes de gouvernance disponibles, stockages et durées de conservation dépendent de la route, de l'intégration et du déploiement retenus.

Un signal de mesure n'autorise pas à lui seul une action. Les mécanismes de blocage, mise en attente, routage ou revue humaine n'existent que lorsque l'intégration consommatrice les implémente et les autorise explicitement.

## 2.3. Options de déploiement souverain

Des modèles de déploiement souverains ou contrôlés peuvent être disponibles selon l'architecture retenue. La localisation des données, les opérateurs, sous-traitants, contrôles d'accès et règles de conservation doivent être documentés pour le déploiement réel ; ils ne se déduisent pas du libellé du déploiement.

# 3. Comment NeoMundi peut contribuer à un processus de conformité à l’AI Act européen

NeoMundi ne remplace ni l’analyse juridique, ni l’évaluation de conformité, ni la gouvernance organisationnelle, ni une certification réglementaire.

Il fournit toutefois des capacités techniques et des preuves en exploitation qui peuvent contribuer à plusieurs domaines opérationnels pertinents dans le cadre d’un processus de conformité à l’AI Act européen.

L’applicabilité de ces domaines dépend du système d’IA concerné, de sa finalité prévue, du rôle de l’organisation, de la classification de risque du système et du cas d’usage spécifique.

| Domaine opérationnel                                | Contribution de NeoMundi                                                                                 | Niveau de couverture                           |
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

Une contribution centrale de NeoMundi réside dans la possibilité de créer un historique longitudinal du comportement observé d’un système d’IA pendant son fonctionnement.

Cela peut aider les organisations à identifier :

* une variation inattendue ;
* une hausse des signaux de risque factuel ;
* des changements de comportement sémantique ;
* une dégradation de la stabilité observée ;
* une évolution de la distribution des risques ;
* des changements de régime silencieux ;
* des schémas nécessitant une revue avant qu’ils ne deviennent visibles par les processus traditionnels de remontée d’incidents.

NeoMundi ne remplace pas une investigation d’incident.

Il aide à établir qu’un signal opérationnel a été observé, mesuré et documenté à un instant donné, dans un contexte défini de mesure et de gouvernance.

---

## 3.2. La distinction entre mesure et autorisation

NeoMundi est conçu autour d’une distinction de gouvernance essentielle :

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

# 4. Comment NeoMundi peut contribuer à un processus de conformité au RGPD

NeoMundi est conçu pour soutenir des principes de traitement des données *privacy-first*.

Il ne remplace ni une analyse complète au regard du RGPD, ni le registre des activités de traitement, ni une analyse d’impact relative à la protection des données, ni la responsabilité juridique du responsable de traitement ou du sous-traitant.

Son architecture peut néanmoins apporter un support technique à plusieurs principes opérationnels liés au RGPD.

| Domaine lié au RGPD                                   | Contribution de NeoMundi                                                                                 | Niveau de couverture                |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | ----------------------------------- |
| Minimisation des données                              | Transmission limitée aux données nécessaires selon le mode et la finalité technique retenus                  | Soutenu par l’architecture          |
| Protection des données dès la conception              | Certains parcours peuvent minimiser l’exposition ; le traitement et la conservation réels dépendent du déploiement                     | Soutenu par l’architecture          |
| Limitation de la conservation                         | Aucune garantie universelle établie ; règles à vérifier pour chaque service, évaluateur, journal, sauvegarde et stockage   | Soutenu par l’architecture          |
| Support à l’accountability                            | Artefacts techniques pouvant aider à documenter les mécanismes de surveillance et de contrôle mis en œuvre   | Contribution opérationnelle directe |
| Traçabilité des contrôles                             | Signaux, métriques, identifiants et historique technique configurable                                        | Techniquement pris en charge        |
| Support à la documentation des traitements            | Éléments techniques pouvant contribuer à la documentation organisationnelle                                  | Contribution partielle              |
| Registre des activités de traitement                  | Document organisationnel et juridique maintenu par le responsable de traitement ou le sous-traitant concerné | Hors périmètre                      |
| Analyse d’impact relative à la protection des données | Évaluation juridique et organisationnelle réalisée lorsqu’elle est requise                                   | Hors périmètre                      |
| Détermination de la base légale                       | Dépend du contexte de traitement et de l’analyse juridique de l’organisation                                 | Hors périmètre                      |
| Gestion des droits des personnes concernées           | Nécessite des procédures et systèmes organisationnels allant au-delà de NeoMundi                         | Hors périmètre                      |

---

# 5. Ce que NeoMundi ne couvre pas

NeoMundi ne remplace pas les responsabilités juridiques, organisationnelles, de sécurité ou de gouvernance d’une organisation.

NeoMundi ne fournit pas :

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

**NeoMundi est une couche de preuve en exploitation, de surveillance continue et de traçabilité pour les réponses générées par des systèmes d’IA.**

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

NeoMundi peut être intégré :

* par un simple appel API ;
* sans nécessiter de modification de l’infrastructure IA sous-jacente ;
* en mode OBS ;
* en mode GOV ;
* selon des modèles de déploiement souverain en fonction de l’architecture retenue ;
* avec des paramètres configurables de surveillance, de seuils, d’alertes et de traçabilité.

Les capacités disponibles dépendent du modèle de déploiement sélectionné, de la profondeur d’intégration et de la configuration de l’organisation.

### Accéder à la plateforme

[**Créer votre compte et votre clé API →**](https://controltower.neomundi.io/welcome)

---

# 8. Avertissement

Ce document décrit les capacités techniques et la contribution opérationnelle visée par NeoMundi.

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

---

## NeoMundi

**Mesure runtime indépendante pour les systèmes d’IA.**

Une primitive de mesure. Plusieurs applications. Plusieurs infrastructures.

**NeoMundi fournit le signal. Votre organisation conserve l’autorité.**
