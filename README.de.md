# UCII

## Universelle Kryptografische Identitätsinfrastruktur

**Identität ist das Fundament. Authentifizierung ist nur eine Anwendung.**

Produktionsreife kryptografische Identitätsinfrastruktur, abgesichert durch Post-Quanten-Kryptografie und wirtschaftlich autorisiert über das x402-Protokoll.

---

## Überblick

UCII (Universelle Kryptografische Identitätsinfrastruktur) ist eine produktionsreife Identitätsinfrastruktur für die nächste Generation des Internets.

Anstatt die Authentifizierung als Grundlage eines Systems zu betrachten, behandelt UCII die **Identität** als dauerhaftes kryptografisches Fundament. Authentifizierung, Autorisierung, Anmeldeinformationen, Zahlungen und anwendungsspezifische Vertrauensmechanismen werden zu Diensten, die auf der Identität aufbauen, anstatt sie zu definieren.

Jede geschützte Operation wird mit moderner Post-Quanten-Kryptografie abgesichert und wirtschaftlich über das x402-Zahlungsprotokoll durchgesetzt.

UCII wurde entwickelt, um eine sichere Grundlage für Menschen, KI-Agenten, autonome Systeme, Organisationen, Dienste und vernetzte Geräte bereitzustellen.

---

## Warum UCII?

Traditionelle Identitätssysteme basieren auf Benutzernamen, Passwörtern, OAuth-Anbietern und Authentifizierungssitzungen.

UCII verfolgt einen anderen Ansatz.

Eine Identität sollte unabhängig davon existieren, wie sie authentifiziert wird.

Passwörter laufen ab.

OAuth-Anbieter ändern sich.

Zertifikate werden erneuert.

Authentifizierungsmethoden entwickeln sich weiter.

Die Identität sollte bestehen bleiben.

UCII etabliert die kryptografische Identität als zentrales Basiselement und ermöglicht es, Authentifizierungsmethoden, Anmeldeinformationen und Autorisierungsmechanismen weiterzuentwickeln, ohne die zugrunde liegende Identität zu ersetzen.

---

## Kernfunktionen

* Universelle kryptografische Identitätsinfrastruktur
* Native Unterstützung mehrerer Identitätsklassen

  * Mensch
  * KI-Agent
  * Gerät
  * Roboter
  * Organisation
  * Dienst
* ML-DSA Post-Quanten-Anmeldeinformationen
* Mehrere aktive Signaturschlüssel
* Sichere Schlüsselrotation
* Kryptografische Überprüfung von Anmeldeinformationen
* Produktionsreife REST-API
* x402-Zahlungsdurchsetzung
* Verifizierung von Zahlungsausgleich (Settlement)
* Dauerhafte Speicherung von Settlement-Belegen
* Schutz vor Replay-Angriffen
* Produktionsreite FastAPI-Bereitstellung

---

## Architektur

```text id="f4nzcn"
               Anwendungen
                     │
             Authentifizierung
                     │
               Autorisierung
                     │
             Anmeldeinformationen
                     │
         Universelle Identität
                     │
      Post-Quanten-Kryptografie
```

Die Identität ist dauerhaft.

Alles andere baut darauf auf.

---

## Wirtschaftliche Autorisierung (x402)

UCII integriert das x402-Protokoll, um eine native wirtschaftliche Autorisierung für Infrastrukturdienste bereitzustellen.

Jeder geschützte Endpoint veröffentlicht den erforderlichen Zahlungsbetrag.

Clients übermitteln einen Zahlungsnachweis.

UCII überprüft den Zahlungsausgleich.

Ein Settlement-Beleg wird dauerhaft gespeichert.

Replay-Versuche werden abgelehnt.

Erst danach wird die geschützte Operation ausgeführt.

Die wirtschaftliche Autorisierung wird damit zu einem festen Bestandteil der Infrastruktur und nicht zu einem externen Abrechnungssystem.

---

## Produktionsstatus

### Phase 2.5 – Produktionsreif abgesichert

✅ Universelle Identitätsinfrastruktur

✅ ML-DSA-Anmeldeinformationssystem

✅ Verifizierung von Anmeldeinformationen

✅ Verifizierung des Zahlungsausgleichs

✅ Dauerhafte Speicherung von Settlement-Belegen

✅ Schutz vor Replay-Angriffen

✅ Produktionstests der Sicherheitsgrenzen

✅ Trennung der Umgebungen

✅ Wirtschaftliche Autorisierung über x402

✅ Öffentliche REST-API

Bereit für die x402-Integration.

---

## Öffentliche API

### Identität erstellen

```text id="r8l7m2"
POST /v1/identity
```

Erstellt eine neue universelle kryptografische Identität.

**Preis:** 0,50 USDC

---

### Anmeldeinformation registrieren

```text id="x0tbmh"
POST /v1/credentials/register
```

Registriert eine kryptografische Anmeldeinformation.

**Preis:** 0,75 USDC

---

### Anmeldeinformation verifizieren

```text id="03r71v"
POST /v1/credentials/verify
```

Überprüft eine registrierte kryptografische Anmeldeinformation.

**Preis:** 0,10 USDC

---

Weitere Endpunkte sind in der OpenAPI-Spezifikation dokumentiert.

---

## Ausrichtung auf Post-Quanten-Sicherheit

UCII basiert auf moderner Post-Quanten-Kryptografie unter Verwendung der vom NIST standardisierten Algorithmen ML-DSA und ML-KEM.

Das Projekt unterstützt den weltweiten Übergang zu quantenresistenter Infrastruktur und soll Organisationen dabei helfen, produktionsreife kryptografische Identitätssysteme rechtzeitig vor den Fristen für die Migration in das Post-Quanten-Zeitalter einzuführen.

---

## Roadmap

### Abgeschlossen

* Universelle kryptografische Identität
* Post-Quanten-Anmeldeinformationen
* Wirtschaftliche Autorisierung über x402
* Verifizierung des Zahlungsausgleichs
* Schutz vor Replay-Angriffen
* Produktionsreife API

### Geplant

* JavaScript SDK
* Python SDK
* Go SDK
* Rust SDK
* Gehostete UCII-Plattform
* Zusätzliche Settlement-Adapter
* Erweiterte Identitätsdienste

---

## Projektvision

UCII entwickelt Infrastruktur – keine einzelne Anwendung.

Identität sollte universell sein.

Kryptografie sollte quantensicher sein.

Autorisierung sollte wirtschaftlich durchsetzbar sein.

Entwickler sollten Anwendungen auf einer Identitätsinfrastruktur aufbauen können, anstatt für jedes Projekt die Identität neu entwickeln zu müssen.

UCII existiert, um genau diese Grundlage bereitzustellen.
