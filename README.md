# Portafolio de Ingeniería de Software: Soluciones Offline-First

**Desarrollador:** Luany Cuesta Rabelo
**Contacto:** luanycuestarabelo@gmail.com | +5358048168
**Telegram:** @Luany92 | **Redes:** Luanyhestia (IG) / Luanyhestia Cuesta (FB)

## Perfil Técnico
Especialista en el diseño y desarrollo de software con arquitectura "Offline-First". Mi enfoque radica en crear soluciones de alta disponibilidad que operan con cero dependencias de servicios en la nube (SaaS), garantizando la continuidad del negocio en entornos de conectividad nula o inestable, optimizando recursos y eliminando costos de infraestructura.

---

## 1. SyncCore: Motor de Sincronización Asíncrona P2P
**El Problema:** La gestión de inventarios y flujo de caja en sucursales distribuidas se paraliza cuando fallan los servidores en la nube o la conexión a internet.
**La Solución:** Un motor de transporte seguro que convierte cualquier estructura de datos o archivo binario en un bloque cifrado transferible por mensajería instantánea (WhatsApp, Telegram, SMS).

**Características Técnicas:**
* **Integridad Criptográfica:** Uso de firmas `HMAC-SHA256` para evitar la alteración o corrupción de paquetes durante el tránsito.
* **Validación Temporal:** Prevención de ataques de repetición (replay attacks) y control de obsolescencia de archivos.
* **Transporte Universal:** Codificación `Base64` acoplada a un esquema JSON estricto para reconstrucción exacta del binario en el destino.

---

## 2. AudioEngine: Motor de Síntesis de Voz Local
**El Problema:** Dependencia de APIs de terceros (como ElevenLabs o Google Cloud TTS) que generan costos por uso, requieren conexión constante y exponen datos.
**La Solución:** Implementación de un sistema *Text-to-Speech* (TTS) integrado y autónomo para generación de activos multimedia.

**Características Técnicas:**
* **Ejecución Concurrente:** Procesamiento de audio encapsulado en hilos (`threading`) para evitar bloqueos en la interfaz gráfica (GUI).
* **Cero Costo Operativo:** Utiliza dependencias nativas del sistema, exportando directamente a `.wav` para integración en pipelines de edición de video, sin latencia de red.

---

## 3. Sistema Integral ERP/POS (En Desarrollo)
*El proyecto principal que integra las tecnologías anteriores.*
Una plataforma completa de gestión de inventario y caja registradora diseñada para operar en hardware de bajos recursos. Incorpora SyncCore para auditorías remotas asíncronas y resolución de conflictos de bases de datos sin servidor central.
