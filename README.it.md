# UCII

## Infrastruttura Universale di Identità Crittografica

**L’identità è il fondamento. L’autenticazione è solo un’applicazione.**

Infrastruttura di identità crittografica pronta per la produzione, protetta dalla Crittografia Post-Quantistica e autorizzata economicamente tramite il protocollo x402.

---

## Panoramica

UCII (Infrastruttura Universale di Identità Crittografica) è un’infrastruttura di identità di livello produttivo progettata per la prossima generazione di Internet.

Invece di considerare l’autenticazione come la base di un sistema, UCII considera **l’identità** come il fondamento crittografico permanente. Autenticazione, autorizzazione, credenziali, pagamenti e meccanismi di fiducia specifici delle applicazioni diventano servizi costruiti sopra l’identità, invece di definirla.

Ogni operazione protetta è salvaguardata utilizzando moderna Crittografia Post-Quantistica e viene applicata economicamente attraverso il protocollo di pagamento x402.

UCII è progettato per fornire una base sicura per persone, agenti IA, sistemi autonomi, organizzazioni, servizi e dispositivi connessi.

---

## Perché UCII?

I sistemi tradizionali di identità ruotano attorno a nomi utente, password, provider OAuth e sessioni di autenticazione.

UCII adotta un approccio differente.

Un’identità dovrebbe esistere indipendentemente dal modo in cui viene autenticata.

Le password scadono.

I provider OAuth cambiano.

I certificati vengono rinnovati.

I metodi di autenticazione evolvono.

L’identità deve rimanere.

UCII stabilisce l’identità crittografica come oggetto radice e consente ai metodi di autenticazione, alle credenziali e ai meccanismi di autorizzazione di evolvere senza sostituire l’identità sottostante.

---

## Funzionalità Principali

* Infrastruttura Universale di Identità Crittografica
* Supporto nativo per molteplici classi di identità

  * Essere umano
  * Agente IA
  * Dispositivo
  * Robot
  * Organizzazione
  * Servizio
* Credenziali crittografiche post-quantistiche ML-DSA
* Molteplici chiavi di firma attive
* Rotazione sicura delle credenziali
* Verifica crittografica delle credenziali
* API REST pronta per la produzione
* Applicazione del protocollo di pagamento x402
* Verifica del settlement
* Persistenza delle ricevute di settlement
* Protezione dagli attacchi di replay
* Distribuzione FastAPI pronta per la produzione

---

## Architettura

```text
                 Applicazioni
                      │
              Autenticazione
                      │
                Autorizzazione
                      │
              Credenziali
                      │
          Identità Universale
                      │
      Crittografia Post-Quantistica
```

L’identità è permanente.

Tutto il resto viene costruito sopra di essa.

---

## Autorizzazione Economica (x402)

UCII integra il protocollo x402 per fornire autorizzazione economica nativa ai servizi infrastrutturali.

Ogni endpoint protetto pubblica il pagamento richiesto.

I client inviano una prova di pagamento.

UCII verifica il settlement.

Una ricevuta di settlement viene registrata permanentemente.

I tentativi di replay vengono rifiutati.

Solo successivamente l’operazione protetta viene eseguita.

L’autorizzazione economica diventa parte dell’infrastruttura invece di dipendere da un sistema esterno di fatturazione.

---

## Stato della Produzione

### Fase 2.5 — Produzione Rafforzata

✅ Infrastruttura Universale di Identità

✅ Framework delle Credenziali ML-DSA

✅ Verifica delle Credenziali

✅ Verifica del Settlement

✅ Persistenza delle Ricevute di Settlement

✅ Protezione Replay

✅ Test dei Confini di Produzione

✅ Separazione degli Ambienti

✅ Autorizzazione Economica tramite x402

✅ API REST Pubblica

Pronto per l’integrazione x402.

---

## API Pubblica

### Creazione Identità

```text
POST /v1/identity
```

Crea una nuova Identità Crittografica Universale.

**Prezzo:** 0,50 USDC

---

### Registrazione Credenziale

```text
POST /v1/credentials/register
```

Registra una credenziale crittografica.

**Prezzo:** 0,75 USDC

---

### Verifica Credenziale

```text
POST /v1/credentials/verify
```

Verifica una credenziale registrata.

**Prezzo:** 0,10 USDC

---

Gli endpoint aggiuntivi sono documentati tramite la specifica OpenAPI.

---

## Allineamento con la Sicurezza Post-Quantistica

UCII è costruito sulla moderna Crittografia Post-Quantistica utilizzando algoritmi standardizzati dal NIST, inclusi ML-DSA e ML-KEM.

Il progetto è allineato alla transizione globale verso infrastrutture resistenti alla computazione quantistica e mira ad aiutare le organizzazioni ad adottare sistemi di identità crittografica pronti per la produzione prima delle scadenze della migrazione post-quantistica.

---

## Roadmap

### Completato

* Identità Crittografica Universale
* Credenziali Post-Quantistiche
* Autorizzazione Economica tramite x402
* Verifica del Settlement
* Protezione Replay
* API di Produzione

### Pianificato

* SDK JavaScript
* SDK Python
* SDK Go
* SDK Rust
* Piattaforma UCII ospitata
* Ulteriori adattatori di settlement
* Espansione dei servizi di identità

---

## Visione del Progetto

UCII sta costruendo infrastruttura, non una semplice applicazione.

L’identità deve essere universale.

La crittografia deve essere resistente alla computazione quantistica.

L’autorizzazione deve essere applicabile economicamente.

Gli sviluppatori devono poter costruire applicazioni sopra un’infrastruttura di identità invece di ricostruire l’identità per ogni nuovo progetto.

UCII esiste per fornire questa base.
