# Python Packages


## Poetry
Dependencies are managed via `poetry` in this project
Please install it via

     curl https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python3 -

The project was initialized with

     poetry new python-packages

and the Virtual Environment was created using

     poetry env use python3

Dependencies are then added with

     poetry add requests

If it is only a dev-dependency you can add the `-D` flag

    poetry add pretty-errors -D


## References
[https://realpython.com/dependency-management-python-poetry/](https://realpython.com/dependency-management-python-poetry/)