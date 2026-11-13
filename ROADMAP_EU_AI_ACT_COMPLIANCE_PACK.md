# NeoMundi — Développement du Pack Conformité EU AI Act
Feuille de route V0.1 • 13 novembre 2026 • Hypothèse produit, non-certifiante

## Objectif et périmètre

Transformer des campagnes Station et des artefacts Evidence en dossiers de preuves techniques vérifiables et lisibles par les équipes conformité et audit. Ne jamais affirmer qu’un pack constitue une certification ou démontre, à lui seul, la conformité d’un système. Cible initiale : un cas d’usage d’IA à haut risque clairement identifié, avec rôle du client (fournisseur/déployeur) et obligations applicables validés.

## Acquis / écarts

Acquis documentés : Station conserve conditions d’exécution, versions, observations, mesures, refus et registres chaînés ; Evidence vérifie archives, intégrité SHA-256, attestations Ed25519/JWS et absences nommées. La chaîne Q-2 a été testée, verdict global PARTIAL. Ce constat documentaire n’équivaut pas à une requalification indépendante du code ou de la production.
Écarts : signaux non entièrement qualifiés scientifiquement ; absence de matrice normative article → obligation → preuve → contrôle ; complétude, rétention, chaîne de conservation et horodatage tiers non garantis de bout en bout ; limites de couverture production et protection des données ; pas de dossier réglementaire prêt à remettre. Les affirmations de détection de dérive dans ai-act-rgpd doivent être alignées sur le démontré.

## Correspondances à instruire

Articles 9 (gestion des risques), 10 (données), 11 (documentation technique), 12 (journaux), 14 (surveillance humaine), 15 (exactitude/robustesse), 17 (qualité), 72 (suivi après commercialisation). Station/Evidence apportent surtout des preuves partielles pour 11–12 ; chaque obligation doit être analysée selon la catégorie d’IA et le rôle du client. Ne pas assimiler une trace d’expérience à la journalisation exhaustive d’un système en production.

## Roadmap par jalons

P0 — Audit opposable : figer versions, spécification et jeux de preuves ; relier chaque affirmation à un chemin Git, test et résultat ; classer DÉMONTRÉ / PARTIEL / NON TESTÉ / ABSENT. Relire le dépôt ai-act-rgpd et corriger les surpromesses.
P1 — Matrice réglementaire versionnée : pour chaque obligation applicable, préciser responsable, preuve attendue, format, méthode de contrôle, couverture, limites, écart et référence au texte officiel. Faire valider l’interprétation juridique.
P2 — Pack V0 : assembler manifest, périmètre, protocole, observations sélectionnées, couverture des évaluateurs, versions, hashes/signatures, résultat du vérificateur, absences explicites, matrice et rapport humain. Formats envisagés : ZIP + JSON/CSV + PDF ; vérification autonome hors ligne.
P3 — Qualification : tests positifs/négatifs, paquets altérés, faux PASS, données manquantes, reproductibilité, confidentialité/RGPD, règles de rétention, accès et gestion des clés. Examen contradictoire par un auditeur externe ; aucun label « conforme » automatique.
P4 — Pilote marché : faire examiner un pack par 2–3 responsables conformité/éditeurs IA ; mesurer temps de préparation, utilité des pièces, lacunes restantes et disposition à payer. Arbitrer seulement ensuite l’industrialisation et la tarification.

## Questions de décision

Quel système et quel rôle réglementaire cibler d’abord ? Quelles preuves exigent réellement les auditeurs ? Qui les signe, les conserve et les vérifie ? Quels flux contiennent des données personnelles ? Quelle durée de conservation ? Comment déclarer NON TESTÉ / NON APPLICABLE sans faux sentiment de conformité ? Qui achète, à quel moment et pour quel gain mesurable ?

## Critère de sortie V0

Un tiers peut ouvrir et vérifier un pack sans NeoMundi, comprendre précisément son périmètre, les preuves présentes, celles qui manquent et les limites scientifiques ; aucune obligation n’est marquée satisfaite sans validation humaine documentée.
Références : règlement (UE) 2024/1689 et modification (UE) 2026/1744 ; dépôts neomundi-station-public, neomundi-evidence-public et ai-act-rgpd. Échéances haut risque : annexe III 02/12/2027 ; annexe I 02/08/2028 (selon régime applicable).

Sources officielles : https://eur-lex.europa.eu/eli/reg/2024/1689/oj ; https://eur-lex.europa.eu/eli/reg/2026/1744/oj
