🌐 **Langues :** [Français](README.md) · [English](README_EN.md)

---

# NeoMundi ControlTower

## Contrôle, traçabilité et contribution aux démarches IA Act et RGPD

NeoMundi a développé **ControlTower**, un instrument de diagnostic, de contrôle continu et de traçabilité conçu pour maîtriser le risque des réponses générées par les systèmes d’intelligence artificielle.

Privacy-first, ControlTower s’intègre sans changement d’infrastructure par simple appel API. La plateforme peut également être déployée en mode souverain.

Ce document présente clairement :

1. ce que ControlTower couvre techniquement aujourd’hui ;
2. ce que la plateforme aide à démontrer dans une démarche IA Act ou RGPD ;
3. ce qui reste à la charge de chaque organisation.

---

# 1. Ce que ControlTower couvre réellement

## 1.1. Traçabilité opérationnelle des réponses IA

ControlTower associe aux réponses observées :

* un identifiant d’observation ;
* des métriques calculées ;
* un score de gouvernance ;
* des signaux de risque exploitables ;
* un historique de mesure configurable ;
* des artefacts de traçabilité adaptés au mode de déploiement.

### Capacité couverte

**Traçabilité technique et opérationnelle des réponses IA observées.**

---

## 1.2. Surveillance continue du risque

ControlTower observe en continu différents signaux liés au comportement des systèmes IA :

* stabilité ;
* cohérence ;
* dérive ;
* risque d’hallucination ;
* validité factuelle lorsque le module correspondant est activé ;
* signaux de risque liés aux réponses générées.

### Capacité couverte

**Monitoring continu du comportement et du risque des réponses IA.**

---

## 1.3. Contrôle continu

ControlTower permet de configurer des règles de gouvernance exploitables en temps réel :

* seuils de risque ;
* alertes ;
* supervision ;
* escalade vers une vérification humaine ;
* blocage ou traitement spécifique des réponses à risque selon l’intégration retenue ;
* audit des observations.

### Capacité couverte

**Contrôle continu du risque des réponses IA.**

---

## 1.4. Auditabilité

ControlTower produit des éléments mesurables et vérifiables :

* métriques ;
* scores ;
* signaux ;
* historique configurable ;
* éléments de justification ;
* artefacts de mesure et de traçabilité.

### Capacité couverte

**Auditabilité des réponses observées et des signaux de risque associés.**

---

## 1.5. Gouvernance fondée sur la preuve

ControlTower ne repose pas uniquement sur une promesse déclarative de fiabilité.

La plateforme fournit des signaux mesurés, traçables et exploitables pour documenter les décisions de contrôle.

### Capacité couverte

**Gouvernance opérationnelle fondée sur des éléments de preuve.**

---

# 2. Une architecture privacy-first

ControlTower est conçu selon les principes suivants :

* **zero content retention** ;
* **zero content logging** ;
* **zero content storage**.

Autrement dit : le contenu des prompts et des réponses n’est ni conservé, ni journalisé, ni stocké par NeoMundi.

Des artefacts minimaux de mesure et de traçabilité peuvent subsister selon le mode choisi et la configuration retenue.

---

## 2.1. Mode OBS

En mode OBS, NeoMundi reçoit uniquement :

* des métriques normalisées ;
* des artefacts techniques d’observation.

NeoMundi ne reçoit pas :

* les prompts ;
* les réponses ;
* le contenu sémantique des échanges.

### Capacité couverte

**Observation du risque sans transmission du contenu.**

---

## 2.2. Mode GOV

En mode GOV, les données transitent en flux temps réel uniquement pour permettre la mesure et l’application des règles de gouvernance.

Le contenu :

* n’est pas conservé ;
* n’est pas indexé ;
* n’est pas réutilisé ;
* n’est pas stocké.

### Capacité couverte

**Contrôle temps réel avec absence de conservation du contenu.**

---

# 3. Ce que ControlTower contribue à démontrer dans une démarche IA Act

ControlTower ne remplace pas une analyse juridique complète et ne délivre pas une certification de conformité.

La plateforme fournit cependant des capacités techniques et des éléments de preuve directement utiles à plusieurs exigences opérationnelles attendues dans une démarche IA Act.

| Domaine                                                  | Contribution de ControlTower                                              | Niveau de couverture                      |
| -------------------------------------------------------- | ------------------------------------------------------------------------- | ----------------------------------------- |
| Surveillance en exploitation                             | Monitoring continu du comportement et du risque des réponses IA           | Couvert techniquement                     |
| Gestion du risque                                        | Scores, signaux, seuils et alertes exploitables                           | Couvert techniquement                     |
| Traçabilité opérationnelle                               | Identifiants d’observation, métriques et artefacts de mesure              | Couvert techniquement                     |
| Journalisation adaptée au risque                         | Historique configurable sans conservation du contenu                      | Couvert techniquement selon configuration |
| Supervision humaine                                      | Seuils, alertes et escalade vers une vérification humaine                 | Capacité technique fournie                |
| Contrôle des réponses à risque                           | Blocage ou traitement spécifique selon l’intégration choisie              | Capacité technique fournie                |
| Auditabilité                                             | Signaux mesurés et éléments de justification                              | Couvert techniquement                     |
| Documentation des incidents                              | Éléments de preuve exploitables pour analyser et documenter les incidents | Contribution directe                      |
| Suivi post-déploiement                                   | Données utiles au monitoring du système en exploitation                   | Contribution directe                      |
| Classification complète du système au regard de l’AI Act | Analyse dépendante du cas d’usage et du rôle de l’organisation            | Hors périmètre                            |

---

# 4. Ce que ControlTower contribue à démontrer dans une démarche RGPD

L’architecture privacy-first de ControlTower contribue directement à plusieurs principes du RGPD.

| Principe                                                            | Contribution de ControlTower                                           | Niveau de couverture     |
| ------------------------------------------------------------------- | ---------------------------------------------------------------------- | ------------------------ |
| Minimisation des données                                            | Transmission limitée au strict nécessaire selon le mode choisi         | Couvert par architecture |
| Protection des données dès la conception                            | Modes OBS et GOV conçus pour limiter l’exposition du contenu           | Couvert par architecture |
| Limitation de la conservation                                       | Zero content retention, zero content logging, zero content storage     | Couvert par architecture |
| Accountability                                                      | Artefacts techniques permettant de démontrer l’existence des contrôles | Contribution directe     |
| Traçabilité des contrôles                                           | Signaux, scores et historique configurable                             | Couvert techniquement    |
| Documentation des traitements                                       | Éléments techniques exploitables par l’organisation                    | Contribution partielle   |
| Registre des traitements                                            | Document organisationnel relevant du responsable de traitement         | Hors périmètre           |
| Analyse d’impact relative à la protection des données — AIPD / DPIA | Analyse juridique et organisationnelle relevant du client              | Hors périmètre           |

---

# 5. Ce que NeoMundi ne couvre pas

NeoMundi ne remplace pas les fonctions juridiques, organisationnelles ou de sécurité de l’entreprise.

ControlTower ne couvre pas :

* la classification juridique complète d’un système au regard de l’AI Act ;
* l’analyse juridique du cas d’usage ;
* la rédaction du registre RGPD ;
* la réalisation d’une AIPD / DPIA ;
* la politique IA interne de l’organisation ;
* la gouvernance RH ;
* la conformité contractuelle ;
* la qualification complète des fournisseurs ;
* la cartographie du Shadow AI ;
* l’audit global de cybersécurité ;
* la certification réglementaire ;
* l’évaluation formelle de conformité.

---

# 6. Positionnement synthétique

**NeoMundi ControlTower est une couche de diagnostic, de contrôle continu et de traçabilité des réponses IA.**

Par architecture, la plateforme fournit des capacités de monitoring, d’auditabilité, de supervision humaine, de gouvernance fondée sur la preuve et de protection des données.

Elle contribue directement à plusieurs exigences opérationnelles attendues dans les démarches IA Act et RGPD, notamment en matière de surveillance, de gestion du risque, de traçabilité et de démonstration des contrôles.

---

# 7. Intégration

ControlTower peut être intégré :

* par simple appel API ;
* sans changement d’infrastructure ;
* en mode OBS ;
* en mode GOV ;
* en mode souverain selon le déploiement retenu.

---

# 8. Avertissement

Ce document présente les capacités techniques de NeoMundi ControlTower.

Il ne constitue pas :

* un avis juridique ;
* une certification réglementaire ;
* une garantie automatique de conformité ;
* une évaluation complète applicable à une organisation ou à un cas d’usage particulier.

La conformité dépend notamment du système concerné, de sa finalité, du contexte d’utilisation, du rôle de l’organisation et des mesures techniques et organisationnelles mises en place.
