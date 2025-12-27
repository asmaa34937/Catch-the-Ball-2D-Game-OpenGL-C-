# Catch the Ball 2D Game (OpenGL/C++)

A classic 2D interactive arcade game built using **C++** and the **OpenGL (GLUT)** library. The project demonstrates core computer graphics concepts, real-time physics, and multi-modal user input handling.

## 🎮 Gameplay Features
* **Real-time Interaction:** Move the basket using the **Mouse** or **Keyboard Arrows** to catch the falling ball.
* **Dynamic Difficulty:** The ball's speed increases gradually as your score rises, making the game more challenging over time.
* **Visual Feedback:** * **Score Tracking:** Real-time score display on the screen.
    * **Game Over State:** High-contrast visual feedback when the player fails to catch the ball.
* **Smooth Rendering:** Utilizes **Double Buffering** to prevent flickering and ensure fluid animations.



## 🛠️ Technical Implementation
* **Graphics API:** OpenGL (Utility Toolkit - GLUT).
* **Collision Detection:** Implemented using axis-aligned bounding box (AABB) logic between the falling sphere and the rectangular basket.
* **Coordinate Mapping:** Transforms pixel-based screen coordinates to world-space coordinates (-2.0 to 2.0) for precise mouse control.
* **Timer Logic:** Managed via `glutTimerFunc` to maintain a consistent frame rate of approximately 60 FPS.

## 🚀 Getting Started

### Prerequisites
* **C++ Compiler** (MinGW, MSVC, or GCC).
* **OpenGL/GLUT Libraries:** Ensure you have `freeglut` or `glut32` installed and linked in your IDE.

### Installation & Run
1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/your-username/catch-the-ball-opengl.git](https://github.com/your-username/catch-the-ball-opengl.git)

   Setup IDE:

        Link opengl32.lib, glu32.lib, and freeglut.lib in your linker settings.

        Place the freeglut.dll in the same folder as your executable.

    Compile and Run: Execute main.cpp using your preferred C++ environment.

⌨️ Controls

    Mouse: Move horizontally to control the basket.

    Left/Right Arrows: Move the basket left or right.

    Home Key / Left Click: Restart the game after a "Game Over".

📊 Project Structure

    main.cpp: Contains the complete game engine, rendering loop, and input handling logic.
