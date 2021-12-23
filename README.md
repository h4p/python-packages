# Python Packages
This is a showroom for awesome Python Packages

## Poetry
Dependencies are managed via `poetry` in this project
Please install it via

     curl https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python3 -

You can then install all required dependencies using

    poetry install

and run tests with

    poetry run pytest


## Poetry setup

The project was initialized with

     poetry new python-packages

and the Virtual Environment was created using

     poetry env use python3

In VSCode you have to add the interpreter path that can be found out with

    poetry env list -v --full-path

Dependencies are then added with

     poetry add requests

If it is only a dev-dependency you can add the `-D` flag

    poetry add pretty-errors -D


## References
[https://realpython.com/dependency-management-python-poetry/](https://realpython.com/dependency-management-python-poetry/)