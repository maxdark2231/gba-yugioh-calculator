# Yu-Gi-Oh! Calculator for GBA / Calculadora de Yu-Gi-Oh! para GBA

Este proyecto es una calculadora de puntos de vida para Yu-Gi-Oh! desarrollada para la consola Game Boy Advance (GBA). Incluye varias funciones como sumar y restar puntos de vida, lanzar un dado, lanzar una moneda, y reiniciar los puntos de vida.

This project is a life point calculator for Yu-Gi-Oh! developed for the Game Boy Advance (GBA) console. It includes several functions like adding and subtracting life points, rolling a die, flipping a coin, and resetting life points.

---

## Funciones Principales / Main Features

- **Sumar y Restar puntos de vida / Add and Subtract Life Points**: Los jugadores pueden seleccionar la cantidad de puntos que desean sumar o restar y aplicarlos a su total de puntos de vida. / Players can select the amount of points they want to add or subtract and apply it to their life point total.
- **Lanzar dado / Roll a Die**: Al presionar el botón L, se lanzará un dado que muestra un número entre 1 y 6. / Press the L button to roll a die that shows a number between 1 and 6.
- **Lanzar moneda / Flip a Coin**: Al presionar el botón R, se lanza una moneda que mostrará "Heads" (cara) o "Tails" (cruz). / Press the R button to flip a coin that will show either "Heads" or "Tails."
- **Reiniciar puntos de vida / Reset Life Points**: Presiona **Start** para reiniciar los puntos de vida de ambos jugadores a 8000. / Press **Start** to reset the life points of both players to 8000.
- **Reiniciar todo / Reset Everything**: Presiona **Select** para reiniciar todo, incluyendo los puntos de vida, la selección de puntos, y los resultados del dado y la moneda. / Press **Select** to reset everything, including life points, point selection, and the die and coin results.

---

## Controles / Controls

- **D-Pad Izquierda/Derecha / Left/Right**: Navega entre las opciones de puntos de vida disponibles (50, 100, 1000, 2000). / Navigate between the available life point options (50, 100, 1000, 2000).
- **D-Pad Arriba/Abajo / Up/Down**: Selecciona entre el Jugador 1 y el Jugador 2. / Select between Player 1 and Player 2.
- **A**: Suma los puntos de vida seleccionados al jugador activo. / Adds the selected life points to the active player.
- **B**: Resta los puntos de vida seleccionados al jugador activo. / Subtracts the selected life points from the active player.
- **L**: Lanza un dado (mostrando un número entre 1 y 6). / Rolls a die (showing a number between 1 and 6).
- **R**: Lanza una moneda (mostrando "Heads" o "Tails"). / Flips a coin (showing "Heads" or "Tails").
- **Start**: Reinicia los puntos de vida de ambos jugadores a 8000. / Resets the life points of both players to 8000.
- **Select**: Reinicia toda la partida, restableciendo los puntos de vida, la selección de puntos, y borrando los resultados del dado y la moneda. / Resets everything, including life points, point selection, and clears the die and coin results.

---

## Tutorial (Español) / Tutorial (English)

### Español

1. **Abrir la Calculadora**:
   - Cuando inicies la calculadora en tu emulador o GBA, verás el título "Yu-Gi-Oh! Calculator" y las instrucciones de uso en la pantalla.
   - Los puntos de vida de los jugadores están configurados a 8000 por defecto.

2. **Seleccionar Puntos para Modificar**:
   - Usa los botones **Izquierda** y **Derecha** en el D-Pad para navegar entre las opciones de puntos disponibles: 50, 100, 1000 y 2000. El valor seleccionado aparecerá resaltado.
   
3. **Seleccionar Jugador**:
   - Usa los botones **Arriba** y **Abajo** para seleccionar entre el Jugador 1 y el Jugador 2.

4. **Sumar o Restar Puntos de Vida**:
   - Una vez que hayas seleccionado un jugador y los puntos que deseas modificar, presiona **A** para sumar los puntos al jugador seleccionado o **B** para restarlos.

5. **Lanzar un Dado**:
   - Presiona **L** para lanzar un dado. El número del dado (1 a 6) aparecerá en la pantalla.

6. **Lanzar una Moneda**:
   - Presiona **R** para lanzar una moneda. Los resultados "Heads" (cara) o "Tails" (cruz) aparecerán en la pantalla.

7. **Reiniciar los Puntos de Vida**:
   - Si deseas reiniciar solo los puntos de vida a 8000, presiona **Start**.

8. **Reiniciar Todo**:
   - Si deseas reiniciar todo (puntos de vida, dado, moneda), presiona **Select**.

---

### English

1. **Open the Calculator**:
   - When you start the calculator on your emulator or GBA, you'll see the title "Yu-Gi-Oh! Calculator" and the usage instructions on the screen.
   - The players' life points are set to 8000 by default.

2. **Select Points to Modify**:
   - Use the **Left** and **Right** buttons on the D-Pad to navigate between the available point options: 50, 100, 1000, and 2000. The selected value will be highlighted.
   
3. **Select a Player**:
   - Use the **Up** and **Down** buttons to select between Player 1 and Player 2.

4. **Add or Subtract Life Points**:
   - Once you've selected a player and the points you want to modify, press **A** to add the points to the selected player or **B** to subtract them.

5. **Roll a Die**:
   - Press **L** to roll a die. The die number (1 to 6) will appear on the screen.

6. **Flip a Coin**:
   - Press **R** to flip a coin. The results "Heads" or "Tails" will appear on the screen.

7. **Reset Life Points**:
   - If you want to reset just the life points to 8000, press **Start**.

8. **Reset Everything**:
   - If you want to reset everything (life points, die, coin), press **Select**.

---

## Detalles del Código / Code Details

### Estructura del Código / Code Structure

El programa está estructurado en varias funciones clave, cada una encargada de una parte específica de la funcionalidad de la calculadora.

The program is structured into several key functions, each responsible for a specific part of the calculator's functionality.

1. **`initTextMode()`**:
   - Inicializa el modo de texto en la pantalla de la GBA. / Initializes the text mode on the GBA screen.

2. **`printStaticScreen()`**:
   - Muestra el título y las instrucciones en la pantalla de inicio. / Displays the title and instructions on the start screen.

3. **`updateLifePoints()`**:
   - Muestra y actualiza los puntos de vida actuales de los jugadores seleccionados en la pantalla. / Displays and updates the current life points of the selected players on the screen.

4. **`showPoints()`**:
   - Muestra las opciones de puntos disponibles y resalta el valor seleccionado. / Displays the available point options and highlights the selected value.

5. **`modifyLifePoints(int add)`**:
   - Modifica los puntos de vida del jugador seleccionado, sumando o restando según el botón presionado (A para sumar, B para restar). / Modifies the selected player's life points, either adding or subtracting depending on the button pressed (A to add, B to subtract).

6. **`rollDice()`**:
   - Simula el lanzamiento de un dado y muestra un número entre 1 y 6. / Simulates rolling a die and displays a number between 1 and 6.

7. **`flipCoin()`**:
   - Simula el lanzamiento de una moneda y muestra "Heads" o "Tails". / Simulates flipping a coin and displays "Heads" or "Tails".

8. **`resetAll()`**:
   - Reinicia los puntos de vida a 8000, limpia los resultados del dado y la moneda, y reinicia las selecciones de puntos. / Resets life points to 8000, clears the die and coin results, and resets the point selections.

---

## Cómo Modificar el Código / How to Modify the Code

1. **Modificar el dado o la moneda / Modify the Die or Coin**:
   - Ajusta la función `rollDice()` para cambiar el rango del dado. / Adjust the `rollDice()` function to change the die range.
   - Edita `flipCoin()` para modificar los resultados de la moneda. / Edit `flipCoin()` to modify the coin results.

2. **Cambiar la disposición de la pantalla / Change Screen Layout**:
   - Usa las funciones `centerText()` y `printLeftText()` para cambiar las posiciones de texto en la pantalla. / Use the `centerText()` and `printLeftText()` functions to change text positions on the screen.

---

## Compilación / Compilation

Para compilar el proyecto, sigue estos pasos:  
To compile the project, follow these steps:

1. Guarda todos los archivos del proyecto en un directorio. / Save all project files in a directory.
2. Asegúrate de tener instalado `devkitPro` con soporte para GBA. / Ensure you have `devkitPro` installed with GBA support.
3. Ejecuta el siguiente comando en el terminal dentro del directorio del proyecto: / Run the following command in the terminal within the project directory:

make
Esto generará un archivo .gba que puedes usar en un emulador o en hardware real de GBA.
This will generate a .gba file that you can use in an emulator or on real GBA hardware.

# Yu-Gi-Oh! Calculator for GBA / Calculadora de Yu-Gi-Oh! para GBA

Este proyecto es una calculadora de puntos de vida para Yu-Gi-Oh! desarrollada para la consola Game Boy Advance (GBA). Incluye varias funciones como sumar y restar puntos de vida, lanzar un dado, lanzar una moneda, y reiniciar los puntos de vida.

This project is a life point calculator for Yu-Gi-Oh! developed for the Game Boy Advance (GBA) console. It includes several functions like adding and subtracting life points, rolling a die, flipping a coin, and resetting life points.

---

## Funciones Principales / Main Features

- **Sumar y Restar puntos de vida / Add and Subtract Life Points**: Los jugadores pueden seleccionar la cantidad de puntos que desean sumar o restar y aplicarlos a su total de puntos de vida. / Players can select the amount of points they want to add or subtract and apply it to their life point total.
- **Lanzar dado / Roll a Die**: Al presionar el botón L, se lanzará un dado que muestra un número entre 1 y 6. / Press the L button to roll a die that shows a number between 1 and 6.
- **Lanzar moneda / Flip a Coin**: Al presionar el botón R, se lanza una moneda que mostrará "Heads" (cara) o "Tails" (cruz). / Press the R button to flip a coin that will show either "Heads" or "Tails."
- **Reiniciar puntos de vida / Reset Life Points**: Presiona **Start** para reiniciar los puntos de vida de ambos jugadores a 8000. / Press **Start** to reset the life points of both players to 8000.
- **Reiniciar todo / Reset Everything**: Presiona **Select** para reiniciar todo, incluyendo los puntos de vida, la selección de puntos, y los resultados del dado y la moneda. / Press **Select** to reset everything, including life points, point selection, and the die and coin results.

---

## Controles / Controls

- **D-Pad Izquierda/Derecha / Left/Right**: Navega entre las opciones de puntos de vida disponibles (50, 100, 1000, 2000). / Navigate between the available life point options (50, 100, 1000, 2000).
- **D-Pad Arriba/Abajo / Up/Down**: Selecciona entre el Jugador 1 y el Jugador 2. / Select between Player 1 and Player 2.
- **A**: Suma los puntos de vida seleccionados al jugador activo. / Adds the selected life points to the active player.
- **B**: Resta los puntos de vida seleccionados al jugador activo. / Subtracts the selected life points from the active player.
- **L**: Lanza un dado (mostrando un número entre 1 y 6). / Rolls a die (showing a number between 1 and 6).
- **R**: Lanza una moneda (mostrando "Heads" o "Tails"). / Flips a coin (showing "Heads" or "Tails").
- **Start**: Reinicia los puntos de vida de ambos jugadores a 8000. / Resets the life points of both players to 8000.
- **Select**: Reinicia toda la partida, restableciendo los puntos de vida, la selección de puntos, y borrando los resultados del dado y la moneda. / Resets everything, including life points, point selection, and clears the die and coin results.

---

## Tutorial (Español) / Tutorial (English)

### Español

1. **Abrir la Calculadora**:
   - Cuando inicies la calculadora en tu emulador o GBA, verás el título "Yu-Gi-Oh! Calculator" y las instrucciones de uso en la pantalla.
   - Los puntos de vida de los jugadores están configurados a 8000 por defecto.

2. **Seleccionar Puntos para Modificar**:
   - Usa los botones **Izquierda** y **Derecha** en el D-Pad para navegar entre las opciones de puntos disponibles: 50, 100, 1000 y 2000. El valor seleccionado aparecerá resaltado.
   
3. **Seleccionar Jugador**:
   - Usa los botones **Arriba** y **Abajo** para seleccionar entre el Jugador 1 y el Jugador 2.

4. **Sumar o Restar Puntos de Vida**:
   - Una vez que hayas seleccionado un jugador y los puntos que deseas modificar, presiona **A** para sumar los puntos al jugador seleccionado o **B** para restarlos.

5. **Lanzar un Dado**:
   - Presiona **L** para lanzar un dado. El número del dado (1 a 6) aparecerá en la pantalla.

6. **Lanzar una Moneda**:
   - Presiona **R** para lanzar una moneda. Los resultados "Heads" (cara) o "Tails" (cruz) aparecerán en la pantalla.

7. **Reiniciar los Puntos de Vida**:
   - Si deseas reiniciar solo los puntos de vida a 8000, presiona **Start**.

8. **Reiniciar Todo**:
   - Si deseas reiniciar todo (puntos de vida, dado, moneda), presiona **Select**.

---

### English

1. **Open the Calculator**:
   - When you start the calculator on your emulator or GBA, you'll see the title "Yu-Gi-Oh! Calculator" and the usage instructions on the screen.
   - The players' life points are set to 8000 by default.

2. **Select Points to Modify**:
   - Use the **Left** and **Right** buttons on the D-Pad to navigate between the available point options: 50, 100, 1000, and 2000. The selected value will be highlighted.
   
3. **Select a Player**:
   - Use the **Up** and **Down** buttons to select between Player 1 and Player 2.

4. **Add or Subtract Life Points**:
   - Once you've selected a player and the points you want to modify, press **A** to add the points to the selected player or **B** to subtract them.

5. **Roll a Die**:
   - Press **L** to roll a die. The die number (1 to 6) will appear on the screen.

6. **Flip a Coin**:
   - Press **R** to flip a coin. The results "Heads" or "Tails" will appear on the screen.

7. **Reset Life Points**:
   - If you want to reset just the life points to 8000, press **Start**.

8. **Reset Everything**:
   - If you want to reset everything (life points, die, coin), press **Select**.

---

## Detalles del Código / Code Details

### Estructura del Código / Code Structure

El programa está estructurado en varias funciones clave, cada una encargada de una parte específica de la funcionalidad de la calculadora.

The program is structured into several key functions, each responsible for a specific part of the calculator's functionality.

1. **`initTextMode()`**:
   - Inicializa el modo de texto en la pantalla de la GBA. / Initializes the text mode on the GBA screen.

2. **`printStaticScreen()`**:
   - Muestra el título y las instrucciones en la pantalla de inicio. / Displays the title and instructions on the start screen.

3. **`updateLifePoints()`**:
   - Muestra y actualiza los puntos de vida actuales de los jugadores seleccionados en la pantalla. / Displays and updates the current life points of the selected players on the screen.

4. **`showPoints()`**:
   - Muestra las opciones de puntos disponibles y resalta el valor seleccionado. / Displays the available point options and highlights the selected value.

5. **`modifyLifePoints(int add)`**:
   - Modifica los puntos de vida del jugador seleccionado, sumando o restando según el botón presionado (A para sumar, B para restar). / Modifies the selected player's life points, either adding or subtracting depending on the button pressed (A to add, B to subtract).

6. **`rollDice()`**:
   - Simula el lanzamiento de un dado y muestra un número entre 1 y 6. / Simulates rolling a die and displays a number between 1 and 6.

7. **`flipCoin()`**:
   - Simula el lanzamiento de una moneda y muestra "Heads" o "Tails". / Simulates flipping a coin and displays "Heads" or "Tails".

8. **`resetAll()`**:
   - Reinicia los puntos de vida a 8000, limpia los resultados del dado y la moneda, y reinicia las selecciones de puntos. / Resets life points to 8000, clears the die and coin results, and resets the point selections.

---

## Cómo Modificar el Código / How to Modify the Code

1. **Modificar el dado o la moneda / Modify the Die or Coin**:
   - Ajusta la función `rollDice()` para cambiar el rango del dado. / Adjust the `rollDice()` function to change the die range.
   - Edita `flipCoin()` para modificar los resultados de la moneda. / Edit `flipCoin()` to modify the coin results.

2. **Cambiar la disposición de la pantalla / Change Screen Layout**:
   - Usa las funciones `centerText()` y `printLeftText()` para cambiar las posiciones de texto en la pantalla. / Use the `centerText()` and `printLeftText()` functions to change text positions on the screen.

---

## Compilación / Compilation

Para compilar el proyecto, sigue estos pasos:  
To compile the project, follow these steps:

1. Guarda todos los archivos del proyecto en un directorio. / Save all project files in a directory.
2. Asegúrate de tener instalado `devkitPro` con soporte para GBA. / Ensure you have `devkitPro` installed with GBA support.
3. Ejecuta el siguiente comando en el terminal dentro del directorio del proyecto: / Run the following command in the terminal within the project directory:

make
Esto generará un archivo .gba que puedes usar en un emulador o en hardware real de GBA.
This will generate a .gba file that you can use in an emulator or on real GBA hardware.

Invítame a un café / Buy Me a Coffee
Si te gusta este proyecto y quieres invitarme a un café, considera hacer una donación de $1:

Donar $1 a través de PayPal

If you like this project and want to buy me a coffee, consider donating $1:

Donate $1 via PayPal




Donate $1 via PayPal

