# get-picture
get picture from websites like 500px, ins sites e.g. 500px, insga

Use flask to build a web-server. It takes original url from the pic website, e.g., 
https://500px.com/photo/221767391/tess-by-peter-coulson?ctx_page=1&from=popular

then, click "get picture". The tool will analyze the webpage, retrive the url for the picture, and display in the same page. E.g., the retrived picture url corresponding to the aforementioned link is https://drscdn.500px.org/photo/221767391/m%3D2048/v2?webp=true&sig=d9458ebaffa124d8cd5cd6daa947e461a1d18352cd067d31d574394f6fc25e71

Requirements:

from flask import Flask, request, render_template

import json

from bs4 import BeautifulSoup

import requests

import re
