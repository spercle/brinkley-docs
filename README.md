Tested on : `Ubunut 22.04`

## Install Prerequisites
```bash

apt install python3-pip
apt install python3.10-venv

apt install libpango-1.0-0 libpangoft2-1.0-0 libcairo2-dev libfreetype6-dev libffi-dev libjpeg-dev libpng-dev libz-dev

sudo apt-get install aspell

python3 -m venv venv/brinkley-docs

source venv/brinkley-docs/bin/activate

pip3 install mkdocs-material mkdocs-with-pdf mkdocs-glightbox mkdocs-material[imaging]


pip install pyspelling

#deactivate when done
deactivate
```

## Create Documentation
```
mkdocs new .
```

## Test
```
mkdocs serve -a 0.0.0.0:8000
```

## Deploy
```
mkdocs gh-deploy
```
##

##
```shell

pyspelling -c .spellcheck/pyspelling.yml -n html

```