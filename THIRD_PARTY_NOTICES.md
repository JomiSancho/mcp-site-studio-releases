# Licencias y procedencia

MCP Site Studio: Copyright (C) 2026 JomiSancho. El código propio se distribuye bajo **AGPL-3.0-only**. Véase LICENSE. Las modificaciones e incorporaciones de esta versión están fechadas y descritas en CHANGELOG.md.

## Unidad de bloques

`qls-mcp-content/includes/class-block-editor.php` y los casos adaptados de `tests/verify-wordpress-blocks.php` conservan **GPL-3.0-only**, seleccionando la versión 3 que permiten sus fuentes GPL-2.0-or-later. No se cambia la concesión original de los respectivos proyectos.

- Stonewright, autor/proyecto `cosmincraciun97/stonewright-wp-mcp`: primitivas e invariantes de árboles/placeholders y casos de direccionamiento. Revisión `3c99cb017c788f045d69e869a04a42abe1b82d24`, `plugin/includes/Support/BlockTree.php` y `plugin/tests/Unit/Gutenberg/BlockAddressingTest.php`. Su LICENSING.md declara GPL-2.0-or-later para plugin y pruebas. No se incorpora el companion MIT, el kernel ni su motor de persistencia.
- GravityKit, proyecto `GravityKit/block-mcp`: guardas de atributos derivados de HTML, bindings/metadata y escenarios de bloques. Revisión `5bdc1e3fa70caddfee078ec8f6b7c49c7a929a9d`, `wordpress-plugin/gk-block-mcp/includes/class-block-writer.php`, `class-block-crud.php` y pruebas relacionadas. La concesión del PHP es GPL-2.0-or-later; la licencia MIT del componente TypeScript no se aplica a esta unidad.

Adaptaciones de 2026-10-16: namespace, rutas por spans del parser nativo, límites, permisos, huellas, preservación de bytes, rechazos de normalización, contrato de propuestas privadas y runner de WordPress del proyecto. Se conserva el aviso de ausencia de garantía de las licencias. La copia GPLv3 está en LICENSE-GPL-3.0.txt.

La combinación de esta unidad GPLv3 con el código AGPLv3 se distribuye conforme a la sección 13 de ambas licencias: las condiciones de cada parte se mantienen y las disposiciones AGPL sobre interacción por red se aplican a la combinación. Referencia: https://www.gnu.org/licenses/license-compatibility.en.html.

## Referencias de diseño y regresiones

Las siguientes fuentes informaron contratos o casos, sin incorporar su servidor, dependencias, tablas, gateways ni motores de recuperación:

- Agent Abilities for MCP (`unaibamir/agent-abilities-for-mcp`), `1cac7f9eeb4a4f8437de20e13c2e66bd7c898c09`, GPL-2.0-or-later: precedencia de clasificación, políticas y casos de invocación denegada/anidada.
- wpmcp (`wpmcp/wpmcp`), `03baa2d71c92606b804bdeffe9e910df4cf73632`, GPL-2.0-or-later: cobertura, truncación y presupuesto de contexto.
- WPVibe (`awesomemotive/wpvibe-ai-mcp`), `62bc77ccd1c15faf766f527a7935fe32f1b227d3`, GPL-2.0-or-later: reconciliación de una respuesta perdida. No se utiliza su gateway alojado.
- EMCP (`msrbuilds/elementor-mcp`), `b17e43d3658d008f4924b9abc216297ff5dfaeaa`, GPL-2.0-or-later: escenarios de fallo del diario y metadata/IDs. Harness y comprobaciones locales son implementación propia.
- Mogacode (`Mogacode-ma/elementor-mcp-agent`), `6001358fa330c866036f3a2181131afd41ff471e`, MIT: predicado de comprobación posterior de una escritura. No se incluye su código TypeScript ni dependencias.

Las APIs de WordPress, MCP Adapter, Rank Math, Elementor y otros proveedores siguen perteneciendo a sus respectivos proyectos. No se incluyen sus paquetes ni código Pro en este ZIP; cada instalación conserva sus requisitos, licencias y cuentas.

## Fuente de la instalación

La herramienta `qls-wordpress/get-plugin-license` y la administración ofrecen una descarga del código instalado para usuarios autenticados de WordPress. Es independiente de la visibilidad de GitHub y contiene únicamente los archivos del plugin y estos documentos. La distribución PHP contiene su fuente editable; no hay un binario propietario ni una suscripción obligatoria del proyecto.
