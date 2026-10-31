# VKT CleanMate

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | [Deutsch](README_de.md) | Español | [Français](README_fr.md)

Ver qué se va a borrar antes de borrarlo. Los sitios de confianza quedan intactos, y de paso te dice en qué se va el tiempo.

> Chrome · Edge · Manifest V3 · Permisos mínimos · Solo local · Sin analítica

Forma parte de la caja de herramientas de privacidad de [VKT](https://www.annmax1983.com/).

---

## ¿Por qué VKT CleanMate?

Casi todos los limpiadores son un único botón de «borrarlo todo». Por eso da miedo encenderlos: un clic y todas las sesiones desaparecen. Y peor: antes de pulsar no sabes si va a tocar 3 sitios o 3000.

VKT CleanMate separa la decisión de la acción.

| Lo que hacen otros limpiadores | El precio |
|---|---|
| Un interruptor que lo borra todo | Un clic equivocado y desaparecen sesiones, cookies e historial de descargas |
| Un diálogo de confirmación sin cifras | No puedes saber si afecta a 3 o a 3000 sitios antes de aceptar |
| Reglas por sitio escondidas tras un campo de regex | Nadie las escribe, así que el modo «seguro» nunca se usa |

| Lo que hace VKT CleanMate | El resultado |
|---|---|
| **Hoja de vista previa en cada ejecución** | Cifras reales del navegador: sitios encontrados, entradas de historial, cookies, tipos activos, ventana de conservación |
| **La versión gratuita no puede borrarlo todo** | Un usuario gratuito no tiene ningún camino hacia el borrado accidental: es diseño, no un aviso |
| **Dos listas en direcciones opuestas** | Lista de limpieza («solo estos», gratis) y lista de protección («estos nunca», de pago) |
| **Los límites se escriben** | En la interfaz y en este README, en lugar de que los descubra un revisor |

En una frase: **ver qué se borra antes de borrar, y saber después en qué se fue el tiempo.**

---

## Funciones

### 🆓 Gratis para siempre

| Función | Qué hace |
|---|---|
| Vista previa | Sitios encontrados, entradas de historial, cookies, tipos de datos y conservación antes de borrar nada |
| Modo dirigido | Limpia solo los dominios de tu lista de limpieza. Entradas ilimitadas |
| Nueve tipos de datos | Historial, caché, cookies, historial de descargas, datos de formularios, almacenamiento local, IndexedDB, service workers y contraseñas guardadas, cada uno con su interruptor |
| Conservación | Mantener la última hora / 3 días / 7 días / 30 días, o todo |
| Cinco disparadores | Al arrancar, al cerrar el navegador, cada N minutos, a diario a una hora fija, tras N minutos inactivo |
| Alcance por disparador | Por ejemplo, historial + caché cada pocas horas y una limpieza profunda con cookies al cerrar |
| Atajos | `Alt+Shift+C` limpiar ahora · `Alt+Shift+X` limpiar y cerrar todas las pestañas y ventanas |
| Postergar | Retrasar la siguiente ejecución automática una hora |
| Notificaciones | Un resumen del resultado tras cada ejecución |
| Seis idiomas | English, 简体中文, 日本語, Deutsch, Español, Français |

### ⭐ Pro (requiere licencia)

| Función | Qué hace |
|---|---|
| Modo completo | Borrar todo excepto tu lista de protección |
| Lista de protección | Los dominios que nunca se tocan; si hay conflicto, gana la protección |
| Huella de enfoque | Tiempo real de enfoque por dominio, distribución de 24 horas, ranking, sugerencias de limpieza |
| Exportación CSV | La huella en CSV, una fila por dominio |

Una licencia cubre dos navegadores. Las funciones gratuitas siguen funcionando cuando la licencia caduca.

---

## Lo que puede y lo que no

### ✅ Puede

- Borrar historial, caché, cookies, descargas, datos de formularios, almacenamiento local, IndexedDB, service workers y contraseñas en cualquier combinación.
- Limitar una limpieza a los dominios que hayas escrito, incluyendo sus subdominios y sin escribir expresiones regulares.
- Saltarse los dominios que proteges, en modo completo.
- Limpiar según un horario, con un alcance de datos distinto por disparador.
- Informar exactamente de lo que se ha eliminado, siempre.

### ❌ No puede

- Borrar cachés DNS, registros del router, registros del proveedor ni logs del servidor. Eso no está en tu dispositivo.
- Restaurar el historial borrado. Chromium no ofrece a ninguna extensión una API para escribirlo de vuelta.
- Limpiar los datos de otro navegador, de otro perfil ni de una copia sincronizada en otro dispositivo.
- Limitar el historial, las descargas, los datos de formularios o las contraseñas a un solo sitio. El navegador no lo expone; esos cuatro tipos se filtran solo en modo completo y la interfaz lo dice junto a la casilla.
- Garantizar el disparador «al cerrar el navegador». Es un mejor esfuerzo: un cierre inesperado, un reinicio forzado o un corte de luz pueden perder esa ejecución.
- Limpiar lo que nunca se guardó. Una página que solo leíste en una ventana privada no deja nada.
- Sustituir a una VPN ni defenderte de la monitorización a nivel de red. Es una herramienta de autoservicio para tu propio navegador en tu propio dispositivo.

---

## Vista previa

> 📸 El material de la tienda está en [`screenshots/`](../screenshots/): cinco capturas de 1280×800 y dos promocionales de 1400×560 y 440×280.

| Captura | Contenido |
|---|---|
| [`01-popup.png`](../screenshots/01-popup.png) | Panel de la barra de herramientas, con el sitio actual ya en la lista de limpieza |
| [`02-preview.png`](../screenshots/02-preview.png) | La hoja de confirmación «Before cleaning» |
| [`03-cleaning.png`](../screenshots/03-cleaning.png) | Ajustes: modo, tipos de datos, conservación, disparadores |
| [`04-lists.png`](../screenshots/04-lists.png) | Ajustes: lista de limpieza y lista de protección |
| [`05-footprint.png`](../screenshots/05-footprint.png) | Página de huella: totales, distribución horaria, ranking |

---

## Navegadores compatibles

| Navegador | Estado |
|---|---|
| Chrome 116+ (escritorio) | ✅ Compatible |
| Microsoft Edge 116+ (escritorio) | ✅ Compatible |
| Otros navegadores Chromium con MV3 | ✅ Debería funcionar |
| Firefox | ❌ No compatible ni previsto |
| Móvil / tableta | ❌ No compatible: no hay barra de herramientas |
| Ventanas privadas | ⚠️ Nada que limpiar: los datos se descartan al cerrar la ventana |

---

## Instalación

**Desde la tienda:** Chrome Web Store o Microsoft Edge Add-ons → «Añadir a Chrome» → fija el icono en la barra.

**Desde el código:**

```bash
npm install          # terser, solo para el empaquetado
npm run build        # dist/ + publish/cleanmate-v<version>.zip
```

Después, `chrome://extensions` → Modo de desarrollador → Cargar descomprimida → esta carpeta (o el `dist/` descomprimido).

---

## Uso

### Primera vez

Abre el panel y pulsa **Limpiar ahora**. Como el modo por defecto es Dirigido y la lista de limpieza está vacía, no pasa nada todavía: ese es el punto. Añade primero un dominio, en el panel para el sitio actual o en la pestaña **Lists**.

### Rellenar la lista de limpieza

- En el panel: **Añadir sitio actual** registra el dominio que estás viendo.
- En la pestaña Lists: escribe `example.com` y pulsa Add. Los subdominios quedan cubiertos y `www.` se elimina solo.
- En la página de huella (Pro): las sugerencias «merece limpieza» y cada fila del ranking tienen un botón que añade el dominio.

### Configurar ejecuciones automáticas

En la pestaña **Cleaning**, cada uno de los cinco disparadores tiene su interruptor. Debajo, un desplegable fija el alcance de datos de ese disparador: `global` sigue las casillas de arriba, cualquier otro valor limita esa ejecución a un preajuste (historial + caché, cookies + caché, todo, etc.).

Un punto de partida razonable: historial + caché cada 6 horas, todo al cerrar el navegador, y dejar arranque e inactividad apagados hasta estar seguro de quererlos.

### Atajos

| Teclas | Acción |
|---|---|
| `Alt+Shift+C` | Limpiar ahora con los ajustes actuales |
| `Alt+Shift+X` | Limpiar ahora y después cerrar todas las pestañas y ventanas |

Ambos se pueden cambiar en `chrome://extensions/shortcuts`.

---

## Cómo funciona

1. Se dispara un activador, o pulsas Limpiar ahora.
2. El service worker de fondo resuelve el ámbito de dominios: tu lista de limpieza en modo dirigido, todo menos la lista de protección en modo completo.
3. Cuenta lo que se vería afectado —sitios, entradas de historial, cookies— y muestra la hoja de vista previa. **Todavía no se ha borrado nada.**
4. Al confirmar, cada tipo de dato seleccionado se elimina mediante `chrome.browsingData`, en lotes de como máximo 50 orígenes.
5. Las reglas de dominio se convierten primero en orígenes reales: `browsingData` acepta orígenes (`https://example.com`) y no nombres de host desnudos, y no expande subdominios por sí mismo.
6. Una notificación informa del resultado, se guarda la marca de tiempo de la ejecución y la hoja sigue accesible desde el panel.

Un detalle de implementación que conviene conocer: `browsingData` solo respeta `origins` para caché, cookies, almacenamiento local, IndexedDB, service workers y sistemas de archivos. El historial, las descargas, los datos de formularios y las contraseñas ignoran por completo esa lista, así que al elegir esos tipos la ejecución abarca todo el perfil. La extensión lo dice en la interfaz en lugar de disimularlo.

---

## Preguntas frecuentes

**¿Limpiar borra mis marcadores?**
No. Los marcadores no forman parte de `browsingData` y ningún código de la extensión los toca.

**¿Borrar cookies me desconectará de todos los sitios?**
En modo dirigido, solo de los dominios de tu lista. Por eso la versión gratuita solo funciona en modo dirigido: un borrado completo es una decisión de pago, tomada a propósito y con la lista de protección en la mano.

**¿Puedo limpiar el historial de un solo sitio?**
Sí. Requiere el permiso opcional `history`, que se pide en el momento de previsualizar o limpiar historial por sitio, no al instalar.

**¿Borra las contraseñas sincronizadas con mi cuenta de Google?**
Si marcas **Contraseñas guardadas**, el navegador elimina el almacén local de contraseñas y un perfil con sesión iniciada puede propagar ese borrado. Ese tipo está desactivado por defecto y marcado en rojo en la interfaz justo por esto. Déjalo apagado salvo que lo quieras de verdad.

**¿Funciona en ventanas privadas?**
Una ventana privada descarta sus datos al cerrarse, así que no queda nada que limpiar. La extensión no necesita acceso a ventanas privadas.

**El disparador «al cerrar el navegador» no se ejecutó.**
Es un mejor esfuerzo. Se dispara cuando el número de ventanas llega a cero; si el navegador se cierra a mitad de la tarea, la limpieza termina unos segundos después del siguiente arranque. Un cierre inesperado, un reinicio forzado o un corte de luz pierden esa ejecución.

**¿Limpia otros navegadores u otros perfiles?**
No. Un perfil, un navegador, este dispositivo.

**¿Por qué la lista de protección es de pago?**
Porque la versión gratuita no puede ejecutar un borrado completo, a propósito. «Borrarlo todo» es la operación arriesgada, y viene con red de seguridad.

---

## Privacidad

Sin analítica, sin telemetría, sin anuncios, sin cuenta. La extensión no lee el contenido de las páginas, no registra pulsaciones y no crea ningún perfil. Los ajustes viven en `chrome.storage.local`. La huella de enfoque, si se activa, guarda dominios, duraciones, número de visitas y una distribución horaria en una ventana móvil de 30 días: sin URL ni títulos. La única petición de red de toda la extensión es la verificación de licencia contra `api.annmax1983.com`, y solo si pegas una clave.

**[📄 Política de privacidad completa](../privacy-policy.html)**

### Permisos

| Permiso | Para qué |
|---|---|
| `browsingData` | Eliminar los tipos de datos que elijas |
| `storage` | Guardar ajustes y la huella opcional en tu dispositivo |
| `alarms` | Programaciones, más un latido por minuto para el cronómetro de enfoque |
| `tabs` | Conocer el dominio actual y actuar sobre la pestaña visible |
| `windows` | Detectar el cierre de la última ventana: la base del disparador «al cerrar» |
| `idle` | El disparador opcional «tras inactividad» |
| `notifications` | El resumen del resultado tras una ejecución |
| `history` *(opcional)* | Solo al previsualizar o limpiar historial por sitio |
| `cookies` *(opcional)* | Solo al limpiar cookies por sitio |
| `api.annmax1983.com` | Únicamente activación y validación de licencia |

Esos dos permisos opcionales son la razón por la que una instalación nueva no muestra el aviso rojo de «leer tu historial de navegación».

---

## Desarrollo

```bash
npm install                   # terser, solo para el empaquetado
npm run icons                 # regenerar icons/*.png (sin dependencias)
npm run build                 # dist/ + publish/cleanmate-v<version>.zip
npm run shoot                 # regenerar screenshots/ en tamaños de tienda
node tools/check-locales.js   # comprobar que los seis idiomas comparten las mismas claves
```

Cargar: `chrome://extensions` → Modo de desarrollador → Cargar descomprimida → esta carpeta.

### Estructura del proyecto

```
manifest.json          MV3, service_worker como módulo ES
background.js          programación, motor de reglas, ejecutor de limpieza, medición de enfoque
license.js             licencia Creem (plugin id: cleanmate)
common/                store (valores por defecto/merge), coincidencia de dominios, i18n, formato, ui.css
popup/                 limpieza en un clic + hoja de vista previa + acciones del sitio actual
options/               modo, tipos de datos, disparadores, listas, interruptor de huella, licencia
insights/              página de huella: solo Pro; mide mientras la página está abierta
_locales/              en, zh_CN, ja, de, es, fr (164 claves cada uno)
languages/             READMEs traducidos
assets/                iconos de UI compartidos
store-listing/         textos de tienda en seis idiomas
index.html             página de aterrizaje (no va en el zip)
promo.html             promocional (objetivo de captura) — 1400×560, `?size=small` da 440×280
screenshots/           capturas de tienda, regeneradas con `npm run shoot`
tools/make-icons.js    generador de iconos PNG sin dependencias
tools/check-locales.js verifica el conjunto de claves de todos los idiomas
tools/shoot.js         renderiza cada superficie en tamaños de tienda
tools/harness/         chrome.* simulado y una página falsa, solo para tools/shoot.js
```

### Sobre el rastreador de enfoque

- Desactivado por defecto y parte de la versión de pago.
- En el modo por defecto solo mide **mientras la página de huella está abierta** (un puerto persistente la mantiene viva). Al cerrarla, deja de medir.
- El service worker no puede usar `setInterval`: las sesiones se cierran con eventos de pestaña o ventana y se completan con una alarma de un minuto.
- Solo se guardan `domain`, `duration`, `visits` y una distribución horaria. Sin URL ni títulos.
- Los usuarios gratuitos ven una tarjeta de licencia en lugar de la página; no se abre ningún puerto, así que no se registra nada.

---

## Aviso de copyright

VKT CleanMate es una herramienta independiente. No está afiliada a Google, Microsoft ni a ningún fabricante de navegadores. Chrome y Edge son marcas de sus respectivos propietarios.

La extensión elimina datos mediante las API del propio navegador. No modifica el navegador, no toca archivos del sistema y no instala nada fuera de su propia carpeta.

---

## Sobre el código fuente

El paquete publicado contiene JavaScript legible, sin ofuscación. `dist/` es la versión compilada y minimizada; el código de este repositorio es su entrada. No se carga nada en remoto: no hay `eval`, ni scripts remotos, ni importaciones dinámicas fuera del propio paquete, lo que impone la política de seguridad de contenido MV3 de `manifest.json`.

---

## ❤️ Apoya el proyecto

**[👉 Obtener una licencia](https://annmax1983.com/extensions/cleanmate)** · **[☕ Invítame a un café](https://ko-fi.com/annmax?ref=vkt-clean-mate)** · [Código en GitHub](https://github.com/annmax1983/vkt-clean-mate) · [Sitio oficial](https://annmax1983.com/)

---

## Licencia

Copyright © 2026 VKT CleanMate. All rights reserved.
