# Developing a Simple Webserver
## NAME: JOHN PAUL J
## REFERENCE NO:23011778
# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using Python code
from http.server import HTTPServer, BaseHTTPRequestHandler
content ="""
<html>
<head>
</head>
<body>
<h1>JOHN PAUL J</h1>
<h1>AIDS</h1>
</body>
</html>
"""

class HelloHandler (BaseHTTPRequestHandler):
   def do_GET (self):
     self.send_response(200)
     self.send_header('Content-type', 'text/html; charset=utf-8')
     self.end.headers ()
     self.wfile.write(content.encode())

server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()

## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
```python   

from http.server import HTTPServer, BaseHTTPRequestHandler
content ="""
<html>
<head>
</head>
<body>
<h1>JOHN PAUL J</h1>
<h1>AIDS<h1>
</body>
</html>
"""

class HelloHandler (BaseHTTPRequestHandler):
   def do_GET (self):
     self.send_response(200)
     self.send_header('Content-type', 'text/html; charset=utf-8')
     self.end.headers ()
     self.wfile.write(content.encode())

server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()
```
# OUTPUT:

![webserver](https://github.com/JOHNSUBIK/ODD2023-WT-Ex-01-Simple-Web-Server/assets/150279319/ce9b06ec-5511-4425-8f94-c39c4d905cd0)


# RESULT:

The program is executed succesfully
