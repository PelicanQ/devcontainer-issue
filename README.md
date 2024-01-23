VSCode Dev Containers issue. Fails to load Python extension

Error from VSCode:

> Cannot activate the 'Black Formatter' extension because it depends on the 'Python' extension, which is not loaded. Would you like to reload the window to load the extension?

To reproduce error:

1. Open a new VSCode window.

1. In Command Palette: Dev Containers: Clone Repository in Container Volume

1. Enter 

1. Open `main.py` and the error dialog should pop up.

