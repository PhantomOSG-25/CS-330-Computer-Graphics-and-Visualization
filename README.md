# CS 330 — Computer Graphics and Visualization

This repository preserves a focused, provenance-safe portion of my CS 330 computer-graphics work. It documents the OpenGL rendering architecture, GLSL shader pipeline, camera controls, mesh infrastructure, and the course framework used to build the final scene.

The current public branch is intentionally **not presented as a complete runnable reproduction of the final visual scene**. Texture assets with unresolved redistribution rights, third-party dependency bundles, generated binaries, and private course artifacts were excluded during portfolio cleanup.

## What this demonstrates

- Understanding a real-time OpenGL rendering loop and scene lifecycle
- Working with model, view, and projection transforms
- Using vertex and fragment shaders for position, normal, texture-coordinate, and lighting calculations
- Navigating a camera with keyboard and mouse input
- Working with reusable mesh and scene-management abstractions
- Evaluating graphics code for attribution, dependencies, portability, and publication risk

## Public branch scope

The public branch contains selected C++ and GLSL files from the verified course project. Several framework files retain their original SNHU instructor attribution. In particular, `MainCode.cpp`, `ViewManager.cpp`, and substantial portions of `SceneManager.cpp` originated from the course framework rather than being wholly student-authored.

`SceneManager.cpp` explicitly marks the methods intended for student modification. The currently published copy contains only a minimal plane-rendering version of those student-editable sections, so this repository should be read as **supporting graphics evidence**, not as one of my primary standalone software projects.

## Source map

- `src/MainCode.cpp` — instructor-provided application/bootstrap framework for GLFW, GLEW, shaders, and the render loop
- `src/ViewManager.*` — instructor-provided camera and view-management framework with keyboard and mouse navigation
- `src/SceneManager.*` — instructor framework plus student-editable scene preparation and rendering sections
- `src/GLMesh.*` — mesh representation and OpenGL buffer helpers retained from the verified project
- `shaders/vertexShader.glsl` — vertex transformation and per-fragment data preparation
- `shaders/fragmentShader.glsl` — material, texture, ambient, diffuse, and specular lighting logic
- `docs/GRAPHICS_REVIEW.md` — architecture, publication decisions, and future improvements
- `RIGHTS.md` — provenance and redistribution notes

## Controls represented in the framework

- `W` / `S` — move the camera forward or backward
- `A` / `D` — move left or right
- Mouse movement — rotate the camera view
- `Esc` — close the window

## Publication and verification status

This branch does not include a complete dependency manifest or cross-platform build configuration, so I do not claim that it can be cloned and built as-is on a clean machine. A fuller portfolio version would require:

1. recovering and reviewing the final student-authored scene sections,
2. confirming redistribution rights for textures and supporting assets,
3. separating instructor framework code from student-authored modifications more clearly,
4. adding a reproducible dependency/build configuration, and
5. validating the reconstructed scene on a clean environment.

Those steps are deliberately left incomplete rather than filling gaps with reconstructed code and presenting it as original coursework.

## Portfolio role

For hiring review, this repository is best used as evidence of graphics coursework and OpenGL familiarity. My stronger standalone engineering projects are the Java service-validation project, Raspberry Pi thermostat, Animal Rescue dashboard, GameAuth service, C++ Course Planner, and Deep Q-Learning Treasure Maze.
