# Making a Bar Chart in D3.js

When testing "1-using-html", "2-using-d3-and-html", and "3-using-svg", you can just open these hmtl files in the browser to test them.
This will cause the browser to use the file:/ scheme to open up html files.

However, when testing "4-using-d3-and-svg", we are loading the external file data.tsv, and the file:/ scheme will throw a 
"Cross origin requests are only supported for HTTP." error. This is because for security reasons, file:/ scheme do not allow
loading of external files.

Hence, we need to load it using the http scheme.

* From the root dir of this project, run *python -m SimpleHTTPServer*
* This starts a webserver, and you can view the html file by going to this url in the browser: *http://localhost:8000/index-4-using-d3-and-svg.html*