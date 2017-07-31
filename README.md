# get-picture
get picture from websites like 500px, instagram, flickr.

Use flask to build a web-server. It takes original url from the pic website. then, click "get picture". The tool will analyze the webpage, retrive the url for the picture, and display in the same page.

How to run program:

1. in terminal, run:
python index.py

2. go to web browser, enter:
http://127.0.0.1:5000/getpic

3. In the textbox, enter the original url from the pic site. Click "get picture" to see the image.

Required lib:
flask, json, BeautifulSoup, requests, re
