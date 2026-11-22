---
title: Política de privacidad — MoneyTracker
lang: es
---

# Política de privacidad — MoneyTracker

**Responsable:** Didier Cruz
**Aplicación:** MoneyTracker (`com.melo.moneytracker`)
**Última actualización:** 22 de noviembre de 2026 (versión 1.9 de la app)

---

## Resumen

**Tus datos financieros nunca salen de tu teléfono.** Toda la información que
registras —cuentas, movimientos, categorías, metas, presupuestos, compras a
cuotas, préstamos y fotos de comprobantes— se guarda **únicamente en el
almacenamiento privado de tu dispositivo**. No existe ningún servidor al que
enviarla: la aplicación no tiene cuentas de usuario y no requiere registro.

**Desde la versión 1.7, la aplicación muestra anuncios** de Google AdMob en
las pantallas Balance y Análisis. Para eso usa internet, y el SDK de anuncios de
Google recopila algunos datos técnicos del dispositivo (no tus finanzas), como
se explica abajo. Quienes ya usaban la aplicación con movimientos registrados
antes de la versión 1.7 no ven anuncios, y en su caso la aplicación no se
comunica con Google.

**Desde la versión 1.9 puedes escanear un ticket o dictar un movimiento.** Las
dos funciones son opcionales y procesan la imagen y la voz **dentro de tu
teléfono**: la foto del ticket, el audio y el texto que se reconoce no se envían
a nadie. Para funcionar, el escaneo usa componentes de Google Play services que
envían a Google métricas técnicas de uso, y el dictado descarga una sola vez un
modelo de reconocimiento de voz desde Hugging Face. Los detalles están abajo.

## Qué datos se recopilan

**Datos financieros: ninguno.** Tus montos, cuentas, categorías, descripciones
y fotos no se envían a nadie, tampoco a la red de anuncios. La aplicación no le
pasa a Google palabras clave ni contenido de tus pantallas para elegir anuncios.

**Datos que recopila el SDK de anuncios de Google** (Google Mobile Ads),
automáticamente, para mostrar anuncios, medirlos (analítica) y prevenir el
fraude:

| Dato | Para qué |
|---|---|
| Dirección IP, de la que se puede deducir la **ubicación aproximada** del dispositivo (ciudad o región, nunca la ubicación exacta) | Elegir anuncios para tu zona y cumplir las leyes de cada país |
| **ID de publicidad** de Android e ID de conjunto de apps | Mostrar anuncios relevantes, limitar cuántas veces ves el mismo y detectar fraude |
| **Interacciones con los anuncios** (si se mostraron o se tocaron) y con la app (por ejemplo, que se abrió) | Medir los anuncios y pagar al desarrollador |
| **Diagnósticos** del rendimiento de la app y del SDK | Que los anuncios funcionen bien y no gasten batería de más |

Google los recibe cifrados en tránsito (TLS) y los trata según su propia
política: [Cómo usa Google la información de los sitios o aplicaciones que
utilizan sus servicios](https://policies.google.com/technologies/partner-sites).
El desarrollador de MoneyTracker **no recibe esos datos**: solo ve en AdMob
totales anónimos, como cuántos anuncios se mostraron y cuánto generaron.

**Datos técnicos del escaneo de tickets (Google ML Kit).** Cuando escaneas un
ticket, la cámara, el recorte del documento y la lectura del texto los hacen
componentes de Google Play services (ML Kit) **dentro de tu teléfono**. La foto
y el texto leído **no se envían a Google ni a nadie**. ML Kit sí envía a Google
métricas de rendimiento y uso de esas funciones: tiempos de respuesta, el
nombre y la versión de la app, códigos de error y la configuración usada. Viajan
cifradas, Google las usa para medir, depurar y mejorar ML Kit y no las comparte
con terceros
([divulgación de datos de ML Kit](https://developers.google.com/ml-kit/android-data-disclosure)).

**Descarga del modelo de dictado (Hugging Face).** La primera vez que usas
«Dictar», la aplicación te avisa del tamaño (unos 57 MB) y, si aceptas, descarga
el modelo de reconocimiento de voz Whisper desde **huggingface.co**. Como en
cualquier descarga, Hugging Face ve tu dirección IP y datos técnicos de la
petición, según su [política de privacidad](https://huggingface.co/privacy).
La descarga no lleva ningún dato tuyo, y después el dictado funciona sin
internet.

**Permisos que declara la aplicación:**

- **Internet y estado de la red:** solo para los anuncios. Sin conexión, la
  app funciona igual y no muestra ningún anuncio.
- **ID de publicidad** (y los permisos de anuncios de Privacy Sandbox de
  Android): para los anuncios, como se explica arriba.
- **Notificaciones:** para los recordatorios de pago que tú activas. Se pide
  solo cuando tiene sentido y puedes negarlo; la app funciona igual.
- **Recibir el aviso de arranque del teléfono:** para que esos recordatorios
  sigan programados tras reiniciarlo. Los recordatorios son **locales**: se
  crean y se muestran en tu teléfono, sin internet.
- **Micrófono:** solo para «Dictar». Se pide la primera vez que tocas «Dictar»,
  después de explicarte para qué, y puedes negarlo; la app funciona igual. El
  audio se guarda unos segundos en un archivo temporal privado, se convierte en
  texto en tu teléfono y **se borra** al terminar. No se graba de forma
  permanente ni se envía a ningún sitio.

La aplicación **no pide acceso a tu ubicación precisa, contactos, cámara ni
almacenamiento externo**. El escaneo de tickets no necesita el permiso de
cámara: la abre el escáner de documentos de Google Play services y la app solo
recibe la imagen escaneada. Puedes comprobar los permisos en la sección
«Permisos de la aplicación» dentro de Google Play.

## Tus opciones sobre los anuncios

- **Si vives en el Espacio Económico Europeo, el Reino Unido o Suiza**, la
  primera vez que abras la aplicación verás el formulario de consentimiento de
  Google. Puedes aceptar o rechazar los anuncios personalizados. Si los
  rechazas, seguirás viendo anuncios, pero sin personalizar. Puedes cambiar tu
  decisión cuando quieras desde el menú lateral, en **«Privacidad de
  anuncios»**.
- **En cualquier país** puedes restablecer o eliminar tu ID de publicidad en
  los ajustes de Android (*Ajustes → Privacidad → Anuncios* o *Google →
  Anuncios*, según el teléfono). Sin ID de publicidad, los anuncios no se
  personalizan.
- **Bloqueamos categorías sensibles** en AdMob: citas, «gane dinero rápido» y
  juegos de casino. Revisamos además los anuncios de apuestas y criptomonedas y
  los bloqueamos cuando aparecen.

Cuando adjuntas la foto de un comprobante, la aplicación no usa la cámara
directamente: le pide a Android que abra **tu aplicación de cámara** o **el
selector de fotos del sistema**, y solo recibe la foto que tú tomas o eliges.
Al escanear un ticket, la aplicación solo recibe la imagen ya escaneada; la
guarda como comprobante del movimiento si tú lo guardas. Lo mismo ocurre con el
respaldo: el archivo se guarda o se abre a través del
**selector de archivos de Android**, en la ubicación que tú escoges. En ningún
caso la aplicación puede ver tus demás fotos ni tus demás archivos.

## Qué datos guarda la aplicación, y dónde

Los datos que tú introduces se almacenan en estos lugares, **todos privados de la
aplicación y dentro de tu propio dispositivo**:

| Qué | Dónde | Contenido |
|---|---|---|
| Tus finanzas | Base de datos local `moneytracker.db` | Cuentas, saldos iniciales, movimientos, categorías, metas, presupuestos, compras a cuotas, préstamos (tasa, cuotas, seguros y cargos), la fecha de tu último respaldo, tus ajustes de recordatorios (hora y tipos de aviso, incluido el recordatorio de respaldo) y si ya completaste la bienvenida |
| Recordatorios programados | Almacenamiento privado de la app | La fecha y el texto de los próximos avisos, para volver a programarlos si reinicias el teléfono |
| Fotos de comprobantes | Carpeta privada de la app | Las fotos que adjuntas a tus movimientos (hasta 6 por movimiento), incluidas las de tickets escaneados |
| Modelo de dictado | Carpeta privada de la app | El modelo de reconocimiento de voz (unos 57 MB), solo si usaste «Dictar». No contiene datos tuyos; se borra al borrar los datos de la app o desinstalarla |
| Archivos temporales | Caché privada de la app | La grabación de un dictado (se borra al convertirla en texto) y la copia de trabajo de un escaneo (se borra al volver a escanear si tiene más de 24 horas, al borrar los datos de la app o cuando Android limpia la caché) |
| Tu preferencia de idioma | Almacenamiento local de la app | Únicamente si elegiste español o inglés |
| Tu decisión sobre anuncios personalizados | Almacenamiento local de la app (lo guarda el SDK de Google) | Solo si te tocó el formulario de consentimiento (Europa, Reino Unido, Suiza) |

Ese almacenamiento es privado: el sistema operativo Android impide que otras
aplicaciones accedan a él. Nadie más puede leerlo, y nosotros tampoco — no
tenemos forma técnica de hacerlo, porque esa información nunca sale de tu
teléfono.

La aplicación tiene además desactivada la copia de seguridad automática de
Android (`allowBackup="false"`), de modo que tus datos financieros tampoco se
copian a los servidores de Google.

## Respaldo de tus datos

Desde la versión 1.2 puedes crear un **archivo de respaldo** con todos tus datos y
tus fotos de comprobantes. Funciona así:

- **Solo se crea cuando tú lo pides**, desde la pantalla Respaldo. La aplicación
  nunca hace respaldos automáticos ni los envía a ningún sitio por su cuenta.
- **Tú decides adónde va.** Puedes guardarlo en una carpeta de tu teléfono o
  compartirlo con la aplicación que elijas (por ejemplo, tu correo o tu servicio
  de almacenamiento en la nube). A partir de ese momento, el archivo queda sujeto
  a las condiciones y la política de privacidad de **esa** aplicación o servicio,
  no de MoneyTracker. Nosotros no recibimos ninguna copia.
- **Contraseña opcional.** Si activas «Proteger con contraseña», el archivo se
  cifra con AES-256 y no se puede abrir sin ella. La contraseña no se guarda en
  ningún lugar: si la olvidas, **nadie puede recuperar ese respaldo**, tampoco
  nosotros. Si no activas la contraseña, cualquiera que obtenga el archivo podrá
  leer su contenido, así que guárdalo en un lugar de confianza.
- **Restaurar** reemplaza los datos de la aplicación por los del archivo que
  elijas. El archivo se lee en tu teléfono; nada se envía a ningún servidor.

## Con quién se comparten tus datos

**Tus datos financieros, con nadie.** La única forma de que salgan de la
aplicación es que tú compartas un archivo de respaldo, como se explica arriba.

**Los datos técnicos de la sección anterior los recibe Google** (Google LLC),
como proveedor de anuncios, y pueden procesarse en servidores fuera de tu país.
Google puede compartirlos con los anunciantes y redes de anuncios con los que
trabaja, según su política y, en Europa, según lo que aceptes en el formulario
de consentimiento.

**Las métricas técnicas de ML Kit** las recibe Google solo si usas el escaneo de
tickets, y **la descarga del modelo de dictado** la atiende Hugging Face solo si
usas «Dictar», como se explica arriba. Ninguna de las dos lleva tus datos
financieros, tus fotos ni tu voz.

Fuera de eso, MoneyTracker no incorpora otros servicios de analítica, informes de errores ni
redes sociales.

## Cuánto tiempo se conservan tus datos, y cómo eliminarlos

Tus datos permanecen en tu dispositivo mientras tú quieras. Como no existe copia
remota en nuestro poder, tienes control completo sobre ellos:

- **Borrar un dato concreto:** elimínalo desde la propia aplicación.
- **Borrar todo de una vez:** Ajustes de Android → Aplicaciones → MoneyTracker →
  Almacenamiento → *Borrar datos*.
- **Desinstalar la aplicación:** Android elimina automáticamente toda la
  información asociada.

Cualquiera de las tres opciones es definitiva e irreversible. **No conservamos
ninguna copia**, así que no hay nada que solicitarnos para que lo borremos.

Los datos técnicos que recibe Google por los anuncios los conserva y elimina
Google según su política. Puedes restablecer o eliminar tu ID de publicidad en
los ajustes de Android, y gestionar tus datos con Google en
[myaccount.google.com](https://myaccount.google.com).

Los **archivos de respaldo** que hayas creado no forman parte de la aplicación:
están donde tú los guardaste o enviaste, y desinstalar la aplicación **no los
borra**. Si quieres eliminarlos, hazlo desde esa carpeta o ese servicio.

## Advertencia importante sobre tus datos

Precisamente porque nada se envía a la nube por sí solo, **si pierdes el
dispositivo, lo restableces de fábrica o desinstalas la app, solo podrás
recuperar tu información si antes creaste un archivo de respaldo y lo guardaste
fuera del teléfono**. La aplicación te muestra la fecha de tu último respaldo
para que sepas qué tan reciente es.

## Menores de edad

MoneyTracker no está dirigida a menores de 13 años. No recopilamos a sabiendas
datos de menores, y los anuncios no están pensados para ellos.

## Tus derechos

Normativas como el RGPD europeo o la CCPA de California reconocen derechos de
acceso, rectificación, eliminación y portabilidad sobre tus datos personales. En
MoneyTracker esos derechos se cumplen por diseño para tus datos financieros: **tú
ya posees todos tus datos, en tu dispositivo, y solo tú puedes consultarlos,
modificarlos o borrarlos.**

Para los datos de anuncios, el responsable es Google: puedes ejercer tus
derechos con Google, retirar o cambiar tu consentimiento desde «Privacidad de
anuncios» (en Europa) y restablecer tu ID de publicidad en los ajustes de
Android. Si tienes dudas, escríbenos y te orientamos.

## Cambios en esta política

Si en el futuro alguna versión de la aplicación modificara su comportamiento —por
ejemplo, incorporando una copia de seguridad automática en la nube o una nueva
red de anuncios—, esta política
se actualizará **antes** de publicar esa versión, y el cambio se indicará de forma
destacada en la descripción de la actualización en Google Play.

**Historial:** 6 de noviembre de 2026 — se añaden las fotos de comprobantes
(versión 1.1), las compras a cuotas y el archivo de respaldo con contraseña
opcional (versión 1.2). 13 de noviembre de 2026 — se añaden los préstamos y
los recordatorios locales de pago, con los permisos de notificaciones y de aviso
de arranque del teléfono (versión 1.6). 18 de noviembre de 2026 — la aplicación
muestra anuncios de Google AdMob y, solo para ellos, usa internet y el ID de
publicidad; tus datos financieros siguen sin salir del teléfono (versión 1.7).
22 de noviembre de 2026 — se añaden el escaneo de tickets y el dictado por voz,
procesados en el teléfono, con el permiso de micrófono, las métricas técnicas de
Google ML Kit y la descarga del modelo de dictado desde Hugging Face; y el
recordatorio local de respaldo (versión 1.9).

## Contacto

Para cualquier duda sobre esta política, escribe a:

**didier.cruz.work@gmail.com**

---

*Esta política describe el comportamiento real de la versión publicada de
MoneyTracker. Los permisos que la aplicación declara pueden revisarse en Google
Play.*
