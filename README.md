# Flappy Bird AI with NEAT

This project is a classic Flappy Bird game where the birds are controlled by a neural network. It uses the **NEAT (NeuroEvolution of Augmenting Topologies)** algorithm to evolve the birds' brains over generations, teaching them to navigate through the pipes.

![Flappy Bird AI Gameplay](https://i.imgur.com/your-gameplay-image.gif)
*(Note: You can replace the link above with a GIF of your actual gameplay)*

---

## Features

* **Classic Gameplay**: Enjoy the familiar Flappy Bird mechanics.
* **AI Control**: Watch as a neural network learns to play the game on its own.
* **NEAT Algorithm**: The project is powered by the NEAT-Python library, which evolves the neural network's topology and weights.
* **Generational Learning**: Observe the AI improve as each new generation learns from the successes and failures of the previous one.
* **Pygame-based**: Built with the popular and easy-to-use Pygame library.

---

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing.

### Prerequisites

* **Python 3.7+** installed on your system.
* **pip** (Python's package installer).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://your-repository-url.git](https://your-repository-url.git)
    cd FLAPPYAI
    ```

2.  **Create and activate a virtual environment (recommended):**
    * **Windows:**
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```
    * **macOS / Linux:**
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```

3.  **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

### Running the Game

To run the simulation and start the AI training process, execute the main script:

```bash
python flappy_bird.py
```

## 🎮 How to Play

The project runs on its own. Your role is to be an observer!

* The simulation starts with a population of birds, each controlled by its own neural network.
* The birds will attempt to fly through the pipes.
* Birds that collide with pipes or the ground are eliminated.
* The simulation continues until all birds are eliminated. The NEAT algorithm then creates a new generation of birds based on the performance of the most successful ones from the previous generation.
* You can monitor the current **Generation** and **Score** at the top of the window.


## 📦 Deployment

You can package this project into a standalone executable file that can be run on other computers without requiring a Python installation.

1.  **Install PyInstaller:**
    ```bash
    pip install pyinstaller
    ```

2.  **Build the executable:**
    * **Windows:**
        ```bash
        pyinstaller --onefile --windowed --add-data "imgs;imgs" --add-data "config-feedforward.txt;." flappy_bird.py
        ```
    * **macOS / Linux:**
        ```bash
        pyinstaller --onefile --windowed --add-data "imgs:imgs" --add-data "config-feedforward.txt:." flappy_bird.py
        ```

3.  The final executable will be located in the `dist/` directory.

# NEAT Algorithm

NEAT (NeuroEvolution of Augmenting Topologies) is an evolutionary algorithm that creates artificial neural networks. It basically takes inspiration from the evolution of life and survival of the fittest.

### Read the research paper given below for understanding the algorithm
[stanley.cec02.pdf](https://github.com/user-attachments/files/18415585/stanley.cec02.pdf)

# Acknowledgement
- [Tech with Tim's Playlist](https://www.youtube.com/watch?v=MMxFDaIOHsE&list=PLzMcBGfZo4-lwGZWXz5Qgta_YNX3_vLS2)
- [Tech with Nikola's Video(Best for visualizing the algorithm)](https://youtu.be/lAjcH-hCusg?si=ixlOyQs8uXCyEa0o)
- [Pygame Documentation](https://www.pygame.org/docs/)

