lecture3notes.md

compphys/
|-- __init__.py
|-- constants.py
|-- physics.py
|-- more/
|   |-- __init__.py
|   |-- morephysics.py
|   |-- evenmorephysics.py
|-- assets/
|   |-- data.txt
|   |-- orphan.py
|-- tests/
|   |-- test_physics.py
|   |-- test_morephysics.py

compphys/	<-----top level module
|-- __init__.py		<--------makes python recognize the module
|-- constants.py	<--------module2 in compphys/
|-- physics.py		<--------module3 in compphys/
|-- more/			<--------submodules in compphys/
|   |-- __init__.py		<-------makes python recognize the submodule
|   |-- morephysics.py
|   |-- evenmorephysics.py
|-- assets/				<-------because no __init__.py, this is simply a directory, not a module
|   |-- data.txt
|   |-- orphan.py
|-- tests/
|   |-- test_physics.py
|   |-- test_morephysics.py


Don't "from ______ import *"; this imports everything into a global namespace, and is not very explicit and you can be using things that you don't know about
You can import modules as shortened things (e.x.: import NumPy as np)

in your __init__ file, you might want to include imports to absolutely key functions to your entire project


pytest finds all files, functions, and modules with the word "test" in them and runs them




