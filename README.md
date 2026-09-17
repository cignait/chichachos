# CHICHACHOS · La Comisión

MVP estático: HTML, CSS y JavaScript, sin instalación ni backend.

## Probar
Desde esta carpeta: `python3 -m http.server 8080`. Abrir http://localhost:8080.

## Publicar
Publicar **solo el contenido de mvp/** en cualquier hosting estático. El archivo de entrada es index.html. No subir la carpeta raíz: contiene el chat privado de WhatsApp. Las fotos de los diez personajes sí forman parte del juego publicado.

## Reglas
Partidas individuales de 180 segundos. Clic/toque sobre una estación para ir y trabajar; también WASD/flechas, E para trabajar y espacio para habilidad. Se necesitan 3 tandas, 3 entregas de hielo y 4 reposeras para aprobar. Cada tanda tarda 14 segundos (Gota 10) y se quema 11 segundos después de estar lista. El apagón permite encender velas del almacén (recuperan visibilidad) o conectar el generador (también restaura refrigeración). Peni trae velas con su habilidad; Gota conecta el generador. Cada error descuenta 60 puntos y reduce temporalmente la velocidad. Las habilidades se recargan en 45 segundos. Pausa manual y automática al ocultar la pestaña.

El patrón diario utiliza la fecha de Argentina. Las habilidades modifican las estrategias; el equilibrio competitivo es provisional. Récord y badges se guardan en localStorage, no se sincronizan ni se verifican en un servidor. Compartir utiliza la función nativa o copia de texto; también hay tarjeta PNG descargable. Sonido opcional sintetizado. Fuentes de Google opcionales con sustitutas locales.

## Alcance
No hay ranking global, cuentas ni multijugador. El puntaje local puede modificarse desde las herramientas del navegador. No hay analíticas. Las fotos son las provistas por el usuario.

## Versión arcade / tutorial
La primera partida abre un tutorial interactivo de seis pasos, sin reloj, enfriamiento ni quemado. También se puede repetir desde Aprender a jugar. Edu activa 8 segundos de velocidad doble y luego una siesta de 2 segundos (19:00 / conexión con Ipa). Los retratos publicados ahora son caricaturas generadas; las fotos originales permanecen en ../characters. El escenario está dibujado en Canvas.

Validación de lógica: desde la raíz del proyecto, `node tests/game.test.cjs`.
