# WebPages for Robot-IA HdF

## Set-up : 

- Install: 

```
git clone git@github.com:robot-ia-hdf/pages.github.io.git robot-ia-hdf
cd robot-ia-hdf
```

- and serve localy: 

```
npx http-server pages
```

You can connect the web site from your favorite web-brother at [http://localhost:8080/](http://localhost:8080/).

## Deployement : 

- Suppose you have configured the public remote: 

```
git remote add public git@github.com:robot-ia-hdf/robot-ia-hdf.github.io.git
git fetch public
git branch --track public public/main
```

- Then: 

```
git checkout public
git merge main
mv README.public.md README.md
git commit -am 'deploy'
git push
```

Anyone can connect the web site from their favorite web-brother at [https://robot-ia-hdf.github.io/](https://robot-ia-hdf.github.io).

