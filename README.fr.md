# UCII

## Infrastructure Universelle d’Identité Cryptographique

**L’identité est le fondement. L’authentification n’est qu’une application.**

Infrastructure d’identité cryptographique prête pour la production, sécurisée par la cryptographie post-quantique et protégée par l’autorisation économique via le protocole x402.

---

## Présentation

UCII (Infrastructure Universelle d’Identité Cryptographique) est une infrastructure d’identité de niveau production conçue pour la prochaine génération d’Internet.

Plutôt que de considérer l’authentification comme le fondement d’un système, UCII considère **l’identité** comme le fondement cryptographique permanent. L’authentification, l’autorisation, les identifiants cryptographiques, les paiements et les mécanismes de confiance propres aux applications deviennent des services construits au-dessus de l’identité, au lieu de la définir.

Chaque opération protégée est sécurisée par une cryptographie post-quantique moderne et appliquée économiquement grâce au protocole de paiement x402.

UCII est conçu pour fournir une base sécurisée aux personnes, aux agents d’IA, aux systèmes autonomes, aux organisations, aux services et aux appareils connectés.

---

## Pourquoi UCII ?

Les systèmes d’identité traditionnels reposent sur les noms d’utilisateur, les mots de passe, les fournisseurs OAuth et les sessions d’authentification.

UCII adopte une approche différente.

Une identité doit exister indépendamment de la manière dont elle est authentifiée.

Les mots de passe expirent.

Les fournisseurs OAuth changent.

Les certificats sont renouvelés.

Les méthodes d’authentification évoluent.

L’identité doit demeurer.

UCII établit l’identité cryptographique comme l’objet fondamental et permet aux méthodes d’authentification, aux identifiants cryptographiques et aux mécanismes d’autorisation d’évoluer sans remplacer l’identité sous-jacente.

---

## Fonctionnalités Principales

* Infrastructure Universelle d’Identité Cryptographique
* Prise en charge native de plusieurs classes d’identité

  * Humain
  * Agent d’IA
  * Appareil
  * Robot
  * Organisation
  * Service
* Identifiants cryptographiques post-quantiques ML-DSA
* Plusieurs clés de signature actives
* Rotation sécurisée des identifiants
* Vérification cryptographique des identifiants
* API REST prête pour la production
* Application du protocole de paiement x402
* Vérification du règlement
* Conservation des reçus de règlement
* Protection contre les attaques par rejeu (Replay)
* Déploiement FastAPI prêt pour la production

---

## Architecture

```text
                 Applications
                      │
              Authentification
                      │
                Autorisation
                      │
            Identifiants cryptographiques
                      │
          Identité Universelle
                      │
      Cryptographie Post-Quantique
```

L’identité est permanente.

Tout le reste repose sur elle.

---

## Autorisation Économique (x402)

UCII intègre le protocole x402 afin de fournir une autorisation économique native pour les services d’infrastructure.

Chaque point de terminaison protégé publie le paiement requis.

Les clients soumettent une preuve de paiement.

UCII vérifie le règlement.

Un reçu de règlement est enregistré de manière permanente.

Les tentatives de rejeu sont rejetées.

Ce n’est qu’ensuite que l’opération protégée est exécutée.

L’autorisation économique devient ainsi une composante native de l’infrastructure plutôt qu’un système de facturation externe.

---

## État de la Production

### Phase 2.5 — Production Renforcée

✅ Infrastructure Universelle d’Identité

✅ Cadre de Gestion des Identifiants ML-DSA

✅ Vérification des Identifiants

✅ Vérification du Règlement

✅ Conservation des Reçus de Règlement

✅ Protection contre les Attaques par Rejeu

✅ Tests des Limites de Production

✅ Séparation des Environnements

✅ Autorisation Économique via x402

✅ API REST Publique

Prêt pour l’intégration avec x402.

---

## API Publique

### Créer une Identité

```text
POST /v1/identity
```

Crée une nouvelle identité cryptographique universelle.

**Prix :** 0,50 USDC

---

### Enregistrer un Identifiant

```text
POST /v1/credentials/register
```

Enregistre un identifiant cryptographique.

**Prix :** 0,75 USDC

---

### Vérifier un Identifiant

```text
POST /v1/credentials/verify
```

Vérifie un identifiant cryptographique enregistré.

**Prix :** 0,10 USDC

---

Les points de terminaison supplémentaires sont documentés dans la spécification OpenAPI.

---

## Conformité avec la Sécurité Post-Quantique

UCII est construit autour d’une cryptographie post-quantique moderne utilisant les algorithmes normalisés par le NIST, notamment ML-DSA et ML-KEM.

Le projet s’inscrit dans la transition mondiale vers des infrastructures résistantes aux ordinateurs quantiques et vise à aider les organisations à adopter des systèmes d’identité cryptographique prêts pour la production avant les échéances de migration vers l’ère post-quantique.

---

## Feuille de Route

### Réalisé

* Identité Cryptographique Universelle
* Identifiants Post-Quantiques
* Autorisation Économique via x402
* Vérification du Règlement
* Protection contre les Attaques par Rejeu
* API de Production

### À venir

* SDK JavaScript
* SDK Python
* SDK Go
* SDK Rust
* Plateforme UCII Hébergée
* Adaptateurs de Règlement Supplémentaires
* Extension des Services d’Identité

---

## Vision du Projet

UCII construit une infrastructure, et non une simple application.

L’identité doit être universelle.

La cryptographie doit être résistante aux ordinateurs quantiques.

L’autorisation doit pouvoir être appliquée de manière économique.

Les développeurs doivent pouvoir construire des applications au-dessus d’une infrastructure d’identité, plutôt que de reconstruire l’identité pour chaque nouveau projet.

UCII existe pour fournir cette fondation.
