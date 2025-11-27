# Recommandations CNIL pour le développement des systèmes d’IA

## Objectif

Ce fichier synthétise les recommandations de la **CNIL** (22 juillet 2025) pour le développement de systèmes d’intelligence artificielle conformes au **RGPD**. Il vise à guider les professionnels (concepteurs, développeurs, DPO, équipes produits…) en conciliant innovation et protection des données.  
[Source CNIL](https://www.cnil.fr/fr/developpement-des-systemes-dia-les-recommandations-de-la-cnil-pour-respecter-le-rgpd)

---

## 1. Contexte et portée

* Ces recommandations concernent les **systèmes d’IA traitant des données personnelles** (apprentissage automatique, IA « générale », systèmes qui continuent d’apprendre).  
* Elles s’appliquent pendant la **phase de développement** : conception, constitution de la base de données, entraînement du modèle.  
* Les recommandations s’articulent avec le **Règlement européen sur l’IA**, en complément du RGPD.

---

## 2. Étapes recommandées pour le développement

### 1. Définir un objectif (finalité)
**Principe :**  
Tout traitement de données personnelles doit avoir une finalité précise, légitime et explicite. Pour un système d’IA, cela consiste à définir clairement le but opérationnel et les résultats attendus.  

**Pratique :**  
- Décrire l’objectif principal et les fonctionnalités attendues.  
- Identifier les données nécessaires et justifier leur utilisation par rapport à l’objectif.  
- Documenter la finalité pour servir de référence tout au long du développement et de l’AIPD.

---

### 2. Déterminer les responsabilités
**Principe :**  
Le RGPD impose de désigner un responsable de traitement et, le cas échéant, un sous-traitant. Dans le contexte IA, il est essentiel de clarifier qui prend les décisions sur les données.  

**Pratique :**  
- Identifier le responsable légal et le responsable opérationnel du projet IA.  
- Définir les rôles : conception, développement, annotation, maintenance.  
- Documenter les responsabilités pour garantir traçabilité et conformité.

---

### 3. Choisir une base légale
**Principe :**  
Tout traitement de données personnelles doit reposer sur une base légale prévue par le RGPD (consentement, intérêt légitime, exécution d’un contrat…).  

**Pratique :**  
- Déterminer la base légale la plus adaptée au projet.  
- Pour le consentement : assurer qu’il est libre, éclairé et spécifique.  
- Pour l’intérêt légitime : réaliser un équilibre entre l’intérêt du responsable et les droits des personnes.  
- Documenter la justification pour l’AIPD et les audits.

---

### 4. Adapter les garanties au moissonnage (web scraping)
**Principe :**  
Les données collectées par moissonnage peuvent soulever des risques particuliers en termes de RGPD, notamment pour l’information des personnes et la proportionnalité du traitement.  

**Pratique :**  
- Identifier les sources et vérifier leur compatibilité avec le RGPD.  
- Prévoir des mesures de sécurité renforcées et limiter la collecte à ce qui est nécessaire.  
- Documenter les efforts pour informer les personnes et respecter leurs droits.  
- Évaluer la pertinence du consentement ou de l’intérêt légitime.

---

### 5. Vérifier la réutilisation des données
**Principe :**  
Les données collectées pour une finalité initiale doivent être compatibles avec la nouvelle finalité de l’IA.  

**Pratique :**  
- Vérifier la compatibilité avec la finalité initiale et la base légale.  
- Supprimer ou anonymiser les données non pertinentes.  
- Documenter les décisions de réutilisation pour justification réglementaire.

---

### 6. Minimiser les données
**Principe :**  
Seules les données strictement nécessaires doivent être utilisées pour l’entraînement, la validation ou les tests du modèle.  

**Pratique :**  
- Limiter le volume et la granularité des données personnelles.  
- Privilégier les données anonymisées ou synthétiques lorsque possible.  
- Mettre en œuvre un suivi de l’utilisation des données et vérifier la pertinence des champs utilisés.  
- Documenter les choix pour faciliter l’AIPD et les audits.

---

### 7. Définir la durée de conservation
**Principe :**  
Les données personnelles ne peuvent pas être conservées indéfiniment.  

**Pratique :**  
- Définir la durée de conservation pour le développement, la maintenance ou l’amélioration du système.  
- Supprimer ou anonymiser les données lorsqu’elles ne sont plus nécessaires.  
- Conserver uniquement les données nécessaires aux audits ou à la mesure des biais avec garanties renforcées.

---

### 8. Informer les personnes concernées
**Principe :**  
Les personnes doivent être informées de l’usage de leurs données et de leurs droits.  

**Pratique :**  
- Fournir une information claire, concise et accessible (formulaire, notice web, schémas).  
- Indiquer les sources, les risques et les mesures de sécurité.  
- Différencier information individuelle et générale selon la proportionnalité.

---

### 9. Assurer l’exercice des droits
**Principe :**  
Permettre aux personnes d’exercer leurs droits sur la base de données ou le modèle.  

**Pratique :**  
- Identifier la personne dans la base ou le modèle, informer des limites techniques.  
- Prévoir réentraînement ou filtres pour respecter les droits.  
- Informer les personnes du délai et des mesures prises.

---

### 10. Sécuriser le système d’IA
**Principe :**  
Mettre en œuvre des mesures techniques et organisationnelles pour protéger les données et le modèle.  

**Pratique :**  
- Confidentialité et intégrité : chiffrement, pseudonymisation, cloisonnement, sauvegardes sécurisées.  
- Fiabilité et performance : audits, librairies vérifiées, contrôle des versions.  
- Fonctionnement anticipé : information utilisateur, filtres sur les sorties, possibilité d’arrêt, watermarking.

---

### 11. Analyser le statut d’un modèle d’IA
**Principe :**  
Vérifier si le modèle contient des données personnelles et relève du RGPD.  

**Pratique :**  
- Tests d’attaques de réidentification si données sensibles ou rares.  
- Mesures possibles : restreindre l’accès, filtrer les sorties, anonymisation, differential privacy.  

---

### 12. Respecter les principes RGPD lors de l’annotation
**Principe :**  
Les annotations doivent respecter la minimisation, l’exactitude et la pertinence des données.  

**Pratique :**  
- Annoter uniquement ce qui est nécessaire pour l’entraînement et la fonctionnalité.  
- Assurer l’exactitude, limiter les biais et éviter les données sensibles sauf exceptions encadrées.  
- Informer des objectifs, mesures de sécurité et responsabilités.

---

## Focus : Analyse d’Impact sur la Protection des Données (AIPD)

**Principe :**  
Évaluer les risques sur la vie privée et planifier des mesures pour les réduire.  

**Quand réaliser une AIPD :**  
- Données sensibles, volume important, personnes vulnérables, croisement de données, usage innovant.  
- Risques élevés : mésusage, divulgation, discrimination, contenu fictif erroné.  

**Mesures correctives :**  
- Sécurité : chiffrement, differential privacy, pseudonymisation.  
- Traçabilité et audits.  
- Gouvernance : comité éthique, documentation.  
- Facilitation de l’exercice des droits : techniques d’explicabilité et traçabilité des sorties.

---

## 3. Autres points importants

* **Check-list CNIL** : validation des principes RGPD (finalité, minimisation, sécurité, gouvernance, droits des personnes).  
* **Intérêt légitime** : conditions pour son utilisation, notamment en cas de moissonnage.  
* **Recommandations à venir** : sécurité, annotation, responsabilités dans la chaîne de valeur.  
* **Outils techniques** : projets comme PANAME pour auditer la confidentialité des modèles.

---

## 4. Liens complémentaires

* [Recommandations CNIL PDF complet](https://www.cnil.fr/sites/cnil/files/2024-04/recommandation_sur_l_application_du_rgpd_au_developpement_des_systemes_d_intelligence_artificielle.pdf)  
* [Liste de vérification CNIL](https://www.cnil.fr/sites/default/files/2025-07/ia_liste_de_verification.pdf)  
* [Recommandations spécifiques pour les bases de données IA](https://www.cnil.fr/fr/developpement-des-systemes-dia-les-recommandations-specifiques)  
* [Finalisation des recommandations et travaux futurs](https://www.cnil.fr/fr/ia-finalisation-recommandations-developpement-des-systemes-ia)

---

## 5. Enjeux et perspectives

* Développer des systèmes d’IA **conformes au RGPD**, conciliant innovation et protection des données.  
* Uniformiser les pratiques dans l’écosystème IA : startups, grandes entreprises, DPO, ingénieurs.  
* Anticiper les obligations futures : statut des modèles IA, responsabilités, outils d’évaluation.

---

*Fin de la synthèse CNIL – pour usage dans le cadre de la veille technologique*
