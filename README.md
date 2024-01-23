## VSCode Dev Containers issue. 
Fails to load Python extension

My system:

- Windows 11 Home

- Docker Desktop 4.26.1 (131620)

- WSL 2 Backend enabled

- VSCode Version: 1.85.2 (user setup)

- VSCode Commit: 8b3775030ed1a69b13e4f4c628c612102e30a681


Error from VSCode:

> Cannot activate the 'Black Formatter' extension because it depends on the 'Python' extension, which is not loaded. Would you like to reload the window to load the extension?

To reproduce error:

1. Open a new VSCode window.

1. In Command Palette: Dev Containers: Clone Repository in Container Volume.

1. Enter `https://github.com/PelicanQ/devcontainer-issue.git`

1. Open `main.py` and the error dialog should pop up.

1. If VSCode has not selected the `defaultInterpreter` as given in `devcontainer.json`, select that Python interpreter and rebuild container. The "... Python, which is not loaded" error remains.
