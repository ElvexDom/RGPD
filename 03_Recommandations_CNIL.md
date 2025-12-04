# Recommandations CNIL pour le développement de l’IA

## Objectif

Ce fichier présente les **recommandations de la CNIL** (22 juillet 2025) pour le développement de systèmes d’IA respectant le **RGPD**, destinées aux concepteurs, développeurs, DPO et équipes produit.

---

## 1. Contexte et portée

- Ciblent les **systèmes d’IA traitant des données personnelles** (apprentissage automatique, IA générale, systèmes continuellement entraînés).  
- Applicables **pendant la phase de développement** : conception, constitution de bases de données, entraînement des modèles.  
- S’articulent avec le **Règlement européen sur l’IA**, en complément du RGPD.

---

## 2. Étapes recommandées pour le développement

### 2.1 Définir un objectif (finalité)

**Principe :** Finalité précise, légitime et explicite pour tout traitement.  

**Pratique :**
- Décrire objectif et fonctionnalités.  
- Identifier données nécessaires et justifier leur utilisation.  
- Documenter la finalité pour référence lors de l’AIPD et des audits.

---

### 2.2 Déterminer les responsabilités

**Principe :** Désigner un responsable de traitement et, si nécessaire, un sous-traitant.  

**Pratique :**
- Identifier responsable légal et opérationnel.  
- Définir les rôles : conception, annotation, maintenance.  
- Documenter pour assurer traçabilité et conformité.

---

### 2.3 Choisir une base légale

**Principe :** Tout traitement de données personnelles doit reposer sur une base légale prévue par le RGPD (consentement, intérêt légitime, contrat, etc.).  

**Pratique :**
- Déterminer la base la plus adaptée.  
- Consentement : libre, éclairé, spécifique.  
- Intérêt légitime : équilibrer intérêts et droits des personnes.  
- Documenter la justification pour AIPD et audits.

---

### 2.4 Adapter les garanties au moissonnage (web scraping)

**Principe :** Les données collectées par moissonnage nécessitent des précautions renforcées.  

**Pratique :**
- Identifier les sources et vérifier compatibilité RGPD.  
- Sécuriser les données et limiter la collecte au nécessaire.  
- Documenter les efforts pour informer les personnes.  
- Évaluer pertinence du consentement ou de l’intérêt légitime.

---

### 2.5 Vérifier la réutilisation des données

**Principe :** Les données initialement collectées doivent être compatibles avec la nouvelle finalité.  

**Pratique :**
- Supprimer ou anonymiser les données non pertinentes.  
- Documenter les décisions de réutilisation pour justification réglementaire.

---

### 2.6 Minimiser les données

**Principe :** Seules les données strictement nécessaires doivent être utilisées.  

**Pratique :**
- Limiter volume et granularité.  
- Favoriser données anonymisées ou synthétiques.  
- Suivre l’utilisation des données et vérifier pertinence des champs utilisés.  
- Documenter les choix pour faciliter AIPD et audits.

---

### 2.7 Définir la durée de conservation

**Principe :** Les données personnelles ne peuvent pas être conservées indéfiniment.  

**Pratique :**
- Définir durée de conservation pour développement, maintenance ou amélioration.  
- Supprimer ou anonymiser les données non nécessaires.  
- Conserver uniquement ce qui est utile aux audits et mesure des biais.

---

### 2.8 Informer les personnes concernées

**Principe :** Les personnes doivent être informées de l’usage de leurs données et de leurs droits.  

**Pratique :**
- Information claire, concise et accessible.  
- Indiquer sources, risques et mesures de sécurité.  
- Différencier information individuelle et générale selon proportionnalité.

---

### 2.9 Assurer l’exercice des droits

**Principe :** Permettre l’exercice des droits sur les données ou le modèle.  

**Pratique :**
- Identifier la personne dans la base ou le modèle.  
- Prévoir réentraînement ou filtres pour respecter les droits.  
- Informer sur délais et mesures prises.

---

### 2.10 Sécuriser le système d’IA

**Principe :** Mettre en œuvre des mesures techniques et organisationnelles pour protéger données et modèles.  

**Pratique :**
- Confidentialité et intégrité : chiffrement, pseudonymisation, cloisonnement, sauvegardes sécurisées.  
- Fiabilité et performance : audits, bibliothèques vérifiées, contrôle des versions.  
- Fonctionnement anticipé : information utilisateur, filtres sur sorties, possibilité d’arrêt, watermarking.

---

### 2.11 Analyser le statut d’un modèle d’IA

**Principe :** Vérifier si le modèle contient des données personnelles et relève du RGPD.  

**Pratique :**
- Tests d’attaques de réidentification pour données sensibles ou rares.  
- Mesures possibles : restreindre accès, filtrer sorties, anonymisation, differential privacy.

---

### 2.12 Respecter les principes RGPD lors de l’annotation

**Principe :** Annotation conforme à minimisation, exactitude et pertinence.  

**Pratique :**
- Annoter uniquement ce qui est nécessaire.  
- Assurer exactitude, limiter biais et éviter données sensibles sauf exceptions.  
- Informer sur objectifs, sécurité et responsabilités.

---

## 3. Analyse d’Impact sur la Protection des Données (AIPD)

**Principe :** Évaluer les risques sur la vie privée et planifier mesures correctives.  

**Quand réaliser une AIPD :**
- Données sensibles, volume important, personnes vulnérables, croisement de données, usage innovant.  
- Risques élevés : mésusage, divulgation, discrimination, contenu fictif erroné.

**Mesures correctives :**
- Sécurité : chiffrement, differential privacy, pseudonymisation.  
- Traçabilité et audits.  
- Gouvernance : comité éthique, documentation.  
- Facilitation des droits : explicabilité, traçabilité des sorties.

---

## 4. Points clés

- Check-list CNIL : validation des principes RGPD (finalité, minimisation, sécurité, gouvernance, droits des personnes).  
- Intérêt légitime : conditions pour son utilisation, notamment lors de moissonnage.  
- Outils techniques : projets comme PANAME pour auditer la confidentialité des modèles.

---

## 5. Sources et références

- [Recommandations CNIL PDF complet](https://www.cnil.fr/sites/cnil/files/2024-04/recommandation_sur_l_application_du_rgpd_au_developpement_des_systemes_d_intelligence_artificielle.pdf)  
- [Liste de vérification CNIL](https://www.cnil.fr/sites/default/files/2025-07/ia_liste_de_verification.pdf)  
- [Recommandations spécifiques pour les bases de données IA](https://www.cnil.fr/fr/developpement-des-systemes-dia-les-recommandations-specifiques)  
- [CNIL – IA et données personnelles](https://www.cnil.fr/fr/reglement-europeen-protection-donnees)  
- [PANAME – CNIL](https://www.cnil.fr/fr/paname-un-partenariat-pour-laudit-de-la-confidentialite-des-modeles-dia)  
- [PEReN – PANAME](https://www.peren.gouv.fr/actualites/2025-06-26_cp_paname/)  

---

[⬅ Retour à la page principale](00_Veille_RGPD_IA.md)
