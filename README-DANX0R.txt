HTTP git server:

./git-smart

LFS:

Trick to see if a LFS server is up:
https://www.theatlantic.com/science/archive/2019/12/when-did-ancient-humans-start-speak/603484/
response: {"message": "403 Forbidden: Your are not authorized to perform this action"}

cat giftless/giftless.yaml 
AUTH_PROVIDERS:
  - giftless.auth.allow_anon:read_write

https://giftless.datopian.com/en/latest/quickstart.html
https://giftless.datopian.com/en/latest/installation.html#running-from-pypi-package

wierd-ass bug fix:
pip install --upgrade Flask-Classful==0.15.0b1

env:
export FLASK_APP=giftless.wsgi_entrypoint

./flask-develop.sh

to create lfs repo:

git lfs track "big/*"
git add .gitattributes
git config lfs.url http://localhost:5000/datahub/testrepo
git lfs ls-files
git remote add origin http://danx0r@localhost:81/danx0r.git

