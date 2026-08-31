# Graphics Engineering Review

## Architecture represented in the public branch

The retained framework initializes GLFW and GLEW, loads GLSL shader stages, creates camera/view and scene managers, and runs a depth-tested render loop. Model, view, and projection matrices connect the scene to the shader pipeline. The fragment shader includes material, texture, ambient, diffuse, and specular-lighting paths.

The current `SceneManager.cpp` public copy renders only a basic plane in its student-editable scene section. It therefore demonstrates the surrounding graphics architecture more strongly than it demonstrates the completed final scene.

## Attribution

The source itself identifies Brian Battersby, SNHU instructor, as the author of multiple framework files. Those files are retained because they establish the course environment in which the project work was completed, but they are not presented as wholly student-authored code.

The portfolio should distinguish among:

- instructor/course framework,
- student-editable sections and project modifications,
- third-party libraries and assets, and
- later portfolio documentation.

## Publication decisions

- Selected verified project source is retained for review.
- Instructor attribution is preserved and made prominent in the README and rights notes.
- Third-party dependency bundles are excluded.
- Texture files are withheld until provenance and redistribution rights are confirmed.
- Generated binaries and Visual Studio state are excluded.
- Screenshots and written assignments remain private supporting evidence pending metadata review.
- The repository is not described as a clean-machine reproducible build because required dependencies and some assets are absent.

## Next improvements

A stronger standalone graphics showcase would require recovering the final student-authored scene changes from the verified schoolwork copy, reviewing each asset for publication rights, separating framework code from student modifications, adding a dependency manifest and cross-platform build configuration, and validating the result in a clean environment.

Until then, this repository is intentionally positioned as supporting evidence of OpenGL and graphics coursework rather than as a flagship application.
