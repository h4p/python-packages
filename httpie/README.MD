# httpie
..is a great package to analyse REST endpoints


## Install
With ``pip install httpie``

## Usage
        
    (venv) > http http://127.0.0.1:8000/snippets/                                    ~/github/django-kata/DjangoExercise(master✗)@twe-mac.local
    HTTP/1.1 200 OK
    Content-Length: 354
    Content-Type: application/json
    Date: Thu, 18 Jun 2020 12:45:30 GMT
    Server: WSGIServer/0.2 CPython/3.8.1
    X-Content-Type-Options: nosniff
    X-Frame-Options: DENY
    
    [
        {
            "code": "foo = \"bar\"\n",
            "id": 1,
            "language": "python",
            "linenos": false,
            "style": "friendly",
            "title": ""
        },
        {
            "code": "print(\"hello, world\")\n",
            "id": 2,
            "language": "python",
            "linenos": false,
            "style": "friendly",
            "title": ""
        },
        {
            "code": "print(\"hello, world\")",
            "id": 3,
            "language": "python",
            "linenos": false,
            "style": "friendly",
            "title": ""
        }
    ]
    
 ## Advanced Example
    (venv) > http --json POST http://127.0.0.1:8000/snippets/ code="print(456)" 
    
    HTTP/1.1 201 Created
    Allow: POST, OPTIONS, GET
    Content-Length: 94
    Content-Type: application/json
    Date: Thu, 18 Jun 2020 13:35:07 GMT
    Server: WSGIServer/0.2 CPython/3.8.1
    Vary: Accept, Cookie
    X-Content-Type-Options: nosniff
    X-Frame-Options: DENY
    
    {
        "code": "print(456)",
        "id": 7,
        "language": "python",
        "linenos": false,
        "style": "friendly",
        "title": ""
    }
 
Add `--debug` to see the request headers