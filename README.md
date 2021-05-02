gustavcaves.github.io
=========

[View Site](https://gustavcaves.github.io/)

Building
--------

```bash
git clone https://github.com/gustavcaves/gustavcaves.github.io.git
cd gustavcaves.github.io
npm install
npm run dev
# Open localhost:4003/index-dev.html in your browser
```

Building for Production
--------

```bash
npm run build
```

From
--------

```bash
STRML.net
```

How to Update with GitHub Console
--------

```bash
git status
npm run build
npm run deploy
git status
git add .
git commit -m "commit"
git status
git push -u origin
```

# Commit

## sunday, 22 de november de 2020 18:03
I have added the public key. From https://pgpkeygen.com/ 


bundle install

bundle exec jekyll serve

base url: "gc_jekyll" in file called _config.yml

git init

git checkout -b gh-pages

git add .

git commit -m "commit test"

git remote add origin https://github.com/gustavcaves/gustavcaves.github.io.git

git push origin gh-pages