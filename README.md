# Kibble Official Website

This project keeps all sources used for building up Kibble official website, served at https://kibble.apache.org.

## Prerequisite
- Python 3 
- Python 3 markdown module (Install by running command `sudo pip3 install markdown`) 

## Build instruction

1. Edit or create the appropriate markdown file in kibble-website/source/ (you can have sub-dirs there) 
2. Open a shell, go to the kibble-website/source/ dir 
3. Run `python3 generate.py` command
4. To verify your change locally, go to kibble-website/content directory 
Run `python -m SimpleHTTPServer 8000` command
The website http://localhost:8000/
5. Commit the changes to git :)


Note: For production site https://kibble.apache.org, the buildbot will regenerate the site from the markdown files and publish it.

