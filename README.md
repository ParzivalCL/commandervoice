# CommanderVoice

Comandos de voz que se traducen a pulsaciones de teclado, como VoiceAttack,
pero reconociendo con [Whisper](https://github.com/openai/whisper) en la tarjeta
gráfica del propio equipo.

**Página del proyecto:** https://parzivalcl.github.io/commandervoice/

Todo corre **en local**: el modelo va dentro del instalador y no sale audio del
equipo. No hay API, no hay cuenta, no hay costo por uso y funciona sin internet.

## Qué hace

Dices *«captura de pantalla»* y el programa pulsa <kbd>Win</kbd>+<kbd>Shift</kbd>+<kbd>S</kbd>.
Los comandos se crean desde la propia ventana: una frase, una tecla.

- **99 idiomas**, detectados en cada frase — puedes dar una orden en español y la
  siguiente en inglés sin tocar nada.
- **Coincidencia difusa**: no hace falta acertar la frase exacta.
- Las teclas se envían por **scancode**, que es lo que necesitan los juegos que
  leen el teclado por DirectInput.
- La interfaz está en español e inglés.

## Requisitos

- Windows 10 u 11 de 64 bits
- Tarjeta **NVIDIA** GTX 16xx / RTX 20xx o posterior, con 4 GB de VRAM y drivers
  527 o superiores
- Un micrófono

La GPU no es opcional en la práctica: el mismo audio tarda **0,43 s** en una
RTX 4060 Ti y **22,3 s** en procesador.

## Descarga

En la [página del proyecto](https://parzivalcl.github.io/commandervoice/) o en
[Releases](https://github.com/ParzivalCL/commandervoice/releases).

## Este repositorio

Contiene la página web del proyecto, publicada con GitHub Pages. El código de la
aplicación no está aquí todavía.
