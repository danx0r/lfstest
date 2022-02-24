HTTP git server:

https://thenewstack.io/how-to-set-up-the-http-git-server-for-private-projects/
install nginx_default as /etc/nginx/sites-available/default


LFS:

https://giftless.datopian.com/en/latest/quickstart.html
https://giftless.datopian.com/en/latest/installation.html#running-from-pypi-package

wierd-ass bug fix:
pip install --upgrade Flask-Classful==0.15.0b1

env:
export FLASK_APP=giftless.wsgi_entrypoint

flask run


to create lfs repo:

git lfs track "big/*"
git add .gitattributes
git config lfs.url http://localhost:5000/datahub/testrepo
git lfs ls-files
git remote add origin http://danx0r@localhost:81/danx0r.git

