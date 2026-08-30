# CS 330 — Computer Graphics and Visualization

This portfolio presents a focused OpenGL scene built in C++ with reusable scene-management code, mesh helpers, GLSL shaders, camera/view controls, lighting, and textured objects.

## What this demonstrates

- Organizing a real-time rendering loop and scene lifecycle
- Modeling reusable meshes and object transforms
- Applying vertex and fragment shaders
- Configuring camera, lighting, materials, and texture coordinates
- Separating view management from scene construction
- Reading and communicating visual design decisions

The source is a focused extraction of the final project. Visual Studio projects, generated binaries, third-party library bulk, and texture assets with unresolved licensing are intentionally excluded pending review.

## Source map

- `src/SceneManager.*` — scene setup, meshes, materials, and lighting
- `src/ViewManager.*` — camera and view controls
- `src/GLMesh.*` — mesh representation and GPU upload helpers
- `src/MainCode.cpp` — application entry point
- `shaders/` — GLSL vertex and fragment stages
