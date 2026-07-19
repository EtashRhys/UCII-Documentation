# UCII

## Infraestructura Universal de Identidad Criptográfica

**La identidad es el elemento fundamental. La autenticación es solo una aplicación.**

Infraestructura de identidad criptográfica lista para producción, protegida mediante criptografía post-cuántica y autorizada económicamente a través del protocolo x402.

---

## Descripción General

UCII (Infraestructura Universal de Identidad Criptográfica) es una infraestructura de identidad de nivel de producción diseñada para la próxima generación de Internet.

En lugar de considerar la autenticación como la base de un sistema, UCII considera la **identidad** como el elemento criptográfico permanente. La autenticación, la autorización, las credenciales, los pagos y los mecanismos de confianza específicos de cada aplicación se convierten en servicios construidos sobre la identidad, en lugar de definirla.

Cada operación protegida se asegura mediante criptografía post-cuántica moderna y se controla económicamente mediante el protocolo de pagos x402.

UCII está diseñado para proporcionar una base segura para personas, agentes de IA, sistemas autónomos, organizaciones, servicios y dispositivos conectados.

---

## ¿Por qué UCII?

Los sistemas tradicionales de identidad giran en torno a nombres de usuario, contraseñas, proveedores OAuth y sesiones de autenticación.

UCII adopta un enfoque diferente.

Una identidad debe existir independientemente de la forma en que se autentica.

Las contraseñas caducan.

Los proveedores OAuth cambian.

Los certificados se renuevan.

Los métodos de autenticación evolucionan.

La identidad debe permanecer.

UCII establece la identidad criptográfica como el objeto raíz y permite que los métodos de autenticación, las credenciales y los mecanismos de autorización evolucionen sin reemplazar la identidad subyacente.

---

## Características Principales

* Infraestructura Universal de Identidad Criptográfica
* Compatibilidad nativa con múltiples clases de identidad

  * Persona
  * Agente de IA
  * Dispositivo
  * Robot
  * Organización
  * Servicio
* Credenciales criptográficas post-cuánticas ML-DSA
* Múltiples claves de firma activas
* Rotación segura de credenciales
* Verificación criptográfica de credenciales
* API REST lista para producción
* Aplicación del protocolo de pagos x402
* Verificación de liquidaciones
* Persistencia de comprobantes de liquidación
* Protección contra ataques de repetición (Replay)
* Despliegue en FastAPI listo para producción

---

## Arquitectura

```text
                Aplicaciones
                      │
              Autenticación
                      │
               Autorización
                      │
                Credenciales
                      │
          Identidad Universal
                      │
     Criptografía Post-Cuántica
```

La identidad es permanente.

Todo lo demás se construye sobre ella.

---

## Autorización Económica (x402)

UCII integra el protocolo x402 para proporcionar autorización económica nativa a los servicios de infraestructura.

Cada endpoint protegido publica el pago requerido.

Los clientes envían una prueba de pago.

UCII verifica la liquidación.

Se registra permanentemente un comprobante de liquidación.

Los intentos de reutilización (Replay) son rechazados.

Solo entonces se ejecuta la operación protegida.

La autorización económica pasa a formar parte de la infraestructura en lugar de depender de un sistema externo de facturación.

---

## Estado de Producción

### Fase 2.5 — Producción Endurecida

✅ Infraestructura Universal de Identidad

✅ Marco de Credenciales ML-DSA

✅ Verificación de Credenciales

✅ Verificación de Liquidaciones

✅ Persistencia de Comprobantes de Liquidación

✅ Protección contra Reutilización (Replay)

✅ Pruebas de Límites de Producción

✅ Separación de Entornos

✅ Autorización Económica mediante x402

✅ API REST Pública

Listo para la integración con x402.

---

## API Pública

### Crear Identidad

```text
POST /v1/identity
```

Crea una nueva Identidad Criptográfica Universal.

**Costo:** 0.50 USDC

---

### Registrar Credencial

```text
POST /v1/credentials/register
```

Registra una credencial criptográfica.

**Costo:** 0.75 USDC

---

### Verificar Credencial

```text
POST /v1/credentials/verify
```

Verifica una credencial registrada.

**Costo:** 0.10 USDC

---

Los endpoints adicionales están documentados mediante la especificación OpenAPI.

---

## Alineación con la Seguridad Post-Cuántica

UCII está construido sobre criptografía post-cuántica moderna utilizando algoritmos estandarizados por NIST, incluyendo ML-DSA y ML-KEM.

El proyecto está alineado con la transición global hacia infraestructuras resistentes a la computación cuántica y tiene como objetivo ayudar a las organizaciones a adoptar sistemas de identidad criptográfica listos para producción antes de los plazos de migración post-cuántica.

---

## Hoja de Ruta

### Completado

* Identidad Criptográfica Universal
* Credenciales Post-Cuánticas
* Autorización Económica mediante x402
* Verificación de Liquidaciones
* Protección contra Reutilización (Replay)
* API de Producción

### Próximamente

* SDK para JavaScript
* SDK para Python
* SDK para Go
* SDK para Rust
* Plataforma UCII alojada
* Adaptadores adicionales de liquidación
* Ampliación de los servicios de identidad

---

## Visión del Proyecto

UCII está construyendo infraestructura, no simplemente una aplicación.

La identidad debe ser universal.

La criptografía debe ser resistente a la computación cuántica.

La autorización debe ser económicamente verificable.

Los desarrolladores deben poder construir aplicaciones sobre una infraestructura de identidad en lugar de reconstruir la identidad para cada proyecto.

UCII existe para proporcionar esa base.


<img width="1200" height="800" alt="17827196299747102586194974612432" src="https://github.com/user-attachments/assets/612b45fc-8b78-4931-a3c9-7d27a1bad07f" />

<p align="center">
  <a href="https://www.whitehouse.gov/gallery/president-donald-j-trump-signs-executive-orders-on-quantum-in-the-oval-office/">
    <img src="https://img.shields.io/badge/White_House-Gallery-0A2540?style=for-the-badge" alt="Gallery">
  </a>
  <a href="https://www.whitehouse.gov/videos/president-trump-signs-executive-orders-jun-22-2026/">
    <img src="https://img.shields.io/badge/Watch-Video-red?style=for-the-badge" alt="Video">
  </a>
  <a href="https://www.youtube.com/live/HNipoXNANAs?si=zfwh6OOjdR42zwA6">
    <img src="https://img.shields.io/badge/YouTube-Live-red?style=for-the-badge&logo=youtube" alt="YouTube">
  </a>
</p>


[![Python](https://img.shields.io/badge/Python-3.11+-blue)](https://www.python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115+-green)](https://fastapi.tiangolo.com)

---

**🛡️ Alineado con las Órdenes Ejecutivas de la Casa Blanca — 22 de junio de 2026**

El 22 de junio de 2026, el Presidente Donald J. Trump firmó dos históricas Órdenes Ejecutivas:

- **EO 14412**: *"Securing the Nation Against Advanced Cryptographic Attacks"*
- **EO 14413**: *"Ushering in the Next Frontier of Quantum Innovation"*

Estas órdenes aceleran la transición de Estados Unidos a la Criptografía Post-Cuántica con plazos agresivos:
- Activos de alto valor e intercambio de claves → **31 de diciembre de 2030**
- Firmas digitales y autenticación → **31 de diciembre de 2031**

---
