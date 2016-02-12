# Simple Web Server

Server the contents of any folder via a simple web server. The SimpleHTTPServer module that comes with Python is a simple HTTP server that provides standard GET and HEAD request handlers. 

Run this in terminal under any folder you want to serve:
```
python -m SimpleHTTPServer
```

Better yet, create an alias in your bash profile:
```
alias www='python -m SimpleHTTPServer'
```

Then using terminal, enter `www` in any folder and go to http://localhost:8000 to see its contents.