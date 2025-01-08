# asteroids

## Installation

We are going to be using pygame and a virtual environment to develop our game.

### Pygame

Pygame is a module for developing games using Python. It provides simple functions and methods for us to easily draw images within a GUI window and handle user input.
Virtual Environment (venv)

Virtual environments are Python's way to keep dependencies (e.g. the pygame module) separate from other projects on our machine. For example, we need pygame version 2 for this project, but another project on your computer might require version 1.

As a best practice, each Python project on your machine should have its own virtual environment to keep them isolated from each other.

Install the Python3-Venv package using the following command:

```
sudo apt install python3.12-venv
```

Create a virtual environment at the top level of your project directory:

```
python3 -m venv venv
```

Activate the virtual environment:

```
source venv/bin/activate
```

You should see (venv) at the beginning of your terminal prompt, for example, mine is:

```
(venv) wagslane@MacBook-Pro-2 asteroids %
```
Note: make sure that your virtual environment is activated when running the game or using the bootdev CLI.

Create a file called requirements.txt in the top level of your project directory with the following contents:

```
pygame==2.6.1
```
This tells Python that this project requires pygame version 2.6.1.

Install the requirements:
```
pip install -r requirements.txt
```
pip is Python's package manager. It will install the pygame module into the virtual environment you created.

Make sure pygame is installed:
```
python3 -m pygame
```
Note: this will result in an error (the test expects an exit code of 1), but the output will show that pygame is installed.

Note: If you are on WSL, you will probably need to install <a href="vcxsrv">VcXsrv</a> to run pygame

[https://vcxsrv.com/wp-content/uploads/2024/09/vcxsrv-64.1.17.2.0.installer.zip](#vcxsrv)




