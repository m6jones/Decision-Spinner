# Decision Wheel & Calm Mode

## Project Overview
**Decision Wheel** is a multi-feature web application designed for both productivity (decision-making) and wellness (relaxation). The project is built as a lightweight, serverless application using modern web standards.

### Main Features
1.  **Decision Wheel (`Spinner.html`)**: An interactive wheel that allows users to create, manage, and spin custom lists of options.
2.  **Rainbow Breath (`Spiral.html`)**: A "Calm Mode" page where users can trace a glowing rainbow spiral with their finger or mouse to practice mindful breathing and relaxation.

### Main Technologies
- **HTML5 & CSS3**: Core structure and styling.
- **Tailwind CSS**: Utility-first styling for a modern, responsive UI.
- **Vanilla JavaScript**: Application logic, state management, and interaction.
- **HTML5 Canvas API**: Used for rendering the interactive wheel and the glowing rainbow trail.
- **Web Storage API (localStorage)**: Persists user lists and options in the Decision Wheel.

### Architecture
The project is a collection of **Single-File Applications (SFAs)**.
- **Decision Wheel**: Manages complex state for multiple lists and utilizes canvas for its primary UI.
- **Calm Mode**: Focuses on high-performance canvas rendering (60fps) and touch/mouse interaction with minimal UI clutter.

## Building and Running
This project does not require a build step or server-side environment.

### Running the Application
1.  **Direct Open**: Open `Spinner.html` to start with the Decision Wheel or `Spiral.html` for Calm Mode.
2.  **Local Server (Optional)**:
    ```bash
    # Example using Python
    python3 -m http.server 8000
    ```
    Navigate to `http://localhost:8000/Spinner.html`.

## Development Conventions
- **Keep it Simple**: Prioritize single-file structures for new features.
- **Visual Polish**: Use Tailwind for layout and Canvas for complex animations.
- **Accessibility**: Ensure touch events are handled alongside mouse events for mobile compatibility.
- **Performance**: Animations (like the spiral trail) should be optimized for smooth 60fps performance using `requestAnimationFrame`.
