# 7. Diseño accesible, animación y asistente de voz

La v2 del prototipo incorpora un sistema de diseño pensado específicamente para personas mayores, más allá de "botones grandes".

## Tipografía
- **Atkinson Hyperlegible** para todo el texto de uso e interfaz: tipografía creada por el Braille Institute específicamente para personas con baja visión, con letras diseñadas para no confundirse entre sí (b/d, 1/l/I, etc.).
- **Fraunces** (serif cálida) reservada solo para títulos, para dar personalidad de marca sin sacrificar legibilidad en el texto funcional.
- Control **A− / A+** visible en la pantalla de inicio: cada persona ajusta el tamaño de letra a su necesidad real, en vez de un tamaño fijo decidido por el equipo. La preferencia se guarda en el dispositivo.

## Paleta
Tonos cálidos inspirados en la lana (ciruela, terracota, salvia, dorado) sobre fondo crema, con contraste alto y sin depender del color como único portador de significado (los estados también cambian de texto, no solo de color).

## Animación
Se usa un único momento de animación no solicitada: en la portada, una línea tipo "punto de tejido" se dibuja al cargar la página. El resto del movimiento en la app responde siempre a una acción del usuario (tocar un botón, cambiar de pantalla, confirmar una acción). Se respeta la preferencia del sistema `prefers-reduced-motion`.

## Asistente de voz
- **Botón flotante de micrófono**, disponible en toda la app. Al activarlo, escucha comandos simples en español ("abrir mi comunidad", "ir al contador", "volver al inicio") y navega automáticamente, confirmando por voz lo que hará.
- **Botón "Escuchar"** en las pantallas con más texto (calculadora, comunidad, círculo familiar), que lee el contenido en voz alta sin necesidad de usar el micrófono.
- Notas técnicas: el reconocimiento de voz depende del navegador (funciona mejor en Chrome) y requiere permiso de micrófono; la lectura en voz alta funciona en la gran mayoría de navegadores modernos.
