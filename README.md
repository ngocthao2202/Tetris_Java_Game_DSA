# Tetris_Java_Game_DSA

## Introduction

The classic video game Tetris, originally developed by Alexey Pajitnov and released in 1984, has been a staple in the gaming community for decades. The game involves players manipulating tetrominoes, geometric shapes composed of four square blocks each, to create horizontal lines without gaps. Completing a line causes it to disappear, and the player earns points while the game gradually increases in speed and difficulty.

In this solo project, I developed a modernized 2D version of Tetris for a course on algorithms & data structures. The game retains the fundamental rules of traditional Tetris. The project emphasizes the application of algorithms and data structures to manage game state and tetromino movements efficiently.

## Objectives

- **Implement Classic Tetris Gameplay**: Recreate the traditional Tetris experience with accurate game mechanics and rules.
- **Enhance Graphics and Sound**: Develop improved visuals and audio effects to create an engaging 2D gaming experience.
- **Introduce New Features**: Add multiple game modes, customizable controls, and dynamic backgrounds to modernize the game.
- **Apply Algorithms and Data Structures**: Utilize advanced algorithms and data structures to manage game state and tetromino movements efficiently.
- **Provide Educational Value**: Use the project as a practical application of concepts learned in the algorithms & data structures course.

## Tools Used

- **Programming and Debugging**: Eclipse
- **Version Control**: GitHub
- **Communication**: Microsoft Teams

## Algorithms

### Game Loop

The game loop updates and draws the screen 60 times per second (60FPS). It uses the `Thread` class to run the game loop.

### Collision Detection Algorithm

The collision detection algorithm checks whether tetromino pieces collide with other pieces or with the boundaries of the game board.

### Line Clearing Algorithm

The line clearing algorithm checks and deletes complete rows when all cells in that row are filled with tetromino pieces.

### Tetromino Movement Algorithm

The tetromino movement algorithm controls the movement of tetromino pieces on the game board, including moving up, down, left, right, and rotating the pieces.

### Auto Drop

The auto drop mechanism automatically lowers the tetromino after a certain period.

### Scoring and Leveling

The scoring and leveling system manages the score, level, and falling rate of tetromino pieces. The score increases as players complete lines, and the level increases along with the falling speed.

### Game Over Conditions

The game over condition checks when the game ends due to no more space for new tetrominoes.

## Data Structures

- **Class Block**: Represents a single block in a tetromino, containing position and color information.
- **Class Mino and Subclasses**: Represent tetrominoes with block arrays to define their shape.
- **Array Blocks**: Contains the blocks of a tetromino, helping to manage the position and status of each block.
- **ArrayList StaticBlocks**: Stores static blocks that have fallen and are no longer moving, used for collision checking and line deletion.
- **Class GamePanel**: Manages the game's graphical interface.
- **Class PlayManager**: Manages gameplay elements such as the current tetromino and the next tetromino.
- **Class KeyHandler**: Manages input from the keyboard.

## Complexity

| Algorithm              | Time Complexity | Space Complexity |
|------------------------|-----------------|------------------|
| Collision Detection    | O(n^2)          | O(1)             |
| Line Clearing          | O(n * m)        | O(1)             |
| Tetromino Movement     | O(1)            | O(1)             |

## Conclusion

The Tetris game project successfully demonstrates the application of fundamental algorithms and data structures in game development. By implementing collision detection, line clearing, and tetromino movement algorithms, the game ensures smooth and accurate gameplay. The use of 2D arrays for the game board and tetromino shapes, along with lists to manage upcoming pieces, highlights efficient data management practices. The project not only provides an engaging gaming experience but also serves as a practical application of concepts learned in algorithms and data structures. This solid foundation enables further enhancements and adaptations, showcasing the versatility and robustness of the implemented solutions.

## Source Code

You can find the complete source code of this project on GitHub:

[GitHub Repository](https://github.com/ngocthao2202/Tetris_Java_Game_DSA)
