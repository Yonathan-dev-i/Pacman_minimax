# Pacman con Algoritmos de Inteligencia Artificial

Este repositorio contiene implementaciones del clásico juego Pacman utilizando tres algoritmos de inteligencia artificial: Expectimax, Minimax y Poda Alfa-Beta. El proyecto está desarrollado en HTML y JavaScript, permitiendo ejecutar los juegos directamente en un navegador web.

# Descripción del Proyecto

El objetivo de este proyecto es demostrar cómo los algoritmos de búsqueda adversarial y probabilística pueden aplicarse a un juego como Pacman. Cada implementación simula un tablero donde Pacman debe recolectar puntos mientras evita ser atrapado por un fantasma. Los algoritmos implementados son:

- Expectimax (Espectimax.html): Utiliza un enfoque probabilístico para modelar el comportamiento del fantasma, que puede ser agresivo (persigue a Pacman) o aleatorio (se mueve sin estrategia). Pacman maximiza su puntuación considerando estas probabilidades.

- Minimax (Minimax.html): Implementa un enfoque clásico de búsqueda adversarial donde Pacman (jugador Max) intenta maximizar su puntuación, mientras el fantasma (jugador Min) intenta minimizarla acercándose a Pacman.

- Poda Alfa-Beta (Poda_alafa_beta.html): Una optimización del algoritmo Minimax que reduce el número de nodos evaluados en el árbol de búsqueda, utilizando valores alpha y beta para podar ramas innecesarias. Incluye estadísticas en tiempo real sobre nodos evaluados y podas realizadas.

# Estructura del Repositorio

- Espectimax.html: Implementación de Pacman con el algoritmo Expectimax. Incluye controles para ajustar la agresividad y aleatoriedad del fantasma.

- Minimax.html: Implementación de Pacman con el algoritmo Minimax en un tablero de 7x7.

- Poda_alafa_beta.html: Implementación de Pacman con el algoritmo de Poda Alfa-Beta, optimizado para una profundidad de búsqueda de 4 niveles.

# Requisitos

- Un navegador web moderno (Chrome, Firefox, Edge, etc.).

- No se requieren dependencias externas, ya que los juegos están implementados completamente en HTML y JavaScript.

# Cómo Ejecutar

Clonar o descargar el repositorio:

git clone https://github.com/Yonathan-dev-i/Pacman_minimax.git

# Abrir los archivos HTML:

- Navega a la carpeta del repositorio (Pacman_minimax).

- Abre cualquiera de los archivos HTML (Espectimax.html, Minimax.html o Poda_alafa_beta.html) en un navegador web. Puedes hacerlo haciendo doble clic en el archivo o usando un servidor local (por ejemplo, con Live Server en VS Code).

# Jugar:

- Haz clic en Iniciar Juego para comenzar.

- Usa los botones Pausar y Reiniciar para controlar el juego.

- En Espectimax.html, ajusta los controles deslizantes para cambiar el comportamiento del fantasma (agresividad y aleatoriedad).

- En Poda_alafa_beta.html, observa las estadísticas de nodos evaluados y podas realizadas durante el juego.

# Detalles de las Implementaciones

Expectimax:

- Tablero: 11x11.

- Profundidad de búsqueda: 3 niveles.

- Características: Comportamiento probabilístico del fantasma, configurable mediante controles deslizantes.

- Evaluación: Basada en la distancia al fantasma, puntos recogidos y cercanía a puntos restantes.

Minimax:

- Tablero: 7x7.

- Profundidad de búsqueda: 3 niveles.

- Características: Pacman maximiza su puntuación, mientras el fantasma intenta atraparlo.

- Evaluación: Basada en la distancia al fantasma, puntos recogidos y puntos restantes.

Poda Alfa-Beta:

- Tablero: 7x7.

- Profundidad de búsqueda: 4 niveles (aumentada gracias a la eficiencia).

- Características: Optimización de Minimax con poda de ramas innecesarias, mostrando estadísticas en tiempo real.

- Evaluación: Similar a Minimax, pero con una bonificación adicional por cercanía a puntos.

# Notas

- Los juegos están diseñados para ejecutarse automáticamente, con Pacman y el fantasma moviéndose según los algoritmos implementados.

- La velocidad del juego es intencionalmente más lenta (1-1.2 segundos por movimiento) para permitir la visualización de los cálculos y el comportamiento del algoritmo.

- El archivo Poda_alafa_beta.html puede tener un nombre con un error tipográfico ("alafa" en lugar de "alfa"). Se recomienda renombrarlo a Poda_alfa_beta.html para mayor claridad.

