# Desarrollo de Proyecto en Ruby 

```bash
# Crear proyecto
rails new nombreProyecto
cd nombreProyecto
# Ejecutar servidor
rails s
```

## Puerto por defecto
```bash
localhost:3000
```

## Posible solución con SQLite en Ruby on rails windows

```bash
gem 'sqlite3', git: "https://github.com/larskanis/sqlite3-ruby", branch: "add-gemspec"
```

## Generando Controller

Nuevo terminal o consola

```bash
rails g controller welcome index

# Archivo routes.rb
get "welcome/index"
root 'welcome#index'
```

## Actualizar gemas

```bash
gem update
gem install rubygems-update
update_rubygems
```

## Borrar Gemfile.lock -> bundler install -> bundle install -> rails s

## Codigos GIT
```bash
# Revisar logs
git log --pretty=oneline
#Cargar cambios y versiones
git branch -M main
git push -u origin main
# Generar Tags
           (Version) 
git tag -a V1.0.0 -m "Mensaje"
git push --tags
#branches (Ramas)
git add .
git checkout -b room
git commit -m "Agregado de dependencias"
git push origin room
#Unir Ramas a main
git checkout main
git merge <Nombre Rama> -m "Mensaje rama"
```

## Subir a Heroku

```
heroku git:clone -a imageniacellphone

# Repetir proceso luego de cambio en el proyecto

git branch
git push heroku main
```

## Crear - borrar variables de entorno Heroku

```
heroku --version
heroku config
heroku config:set nombre="Guillermo"
heroku config:unset nombre
```

## Logs en heroku

```
heroku logs -n 100 -a
heroku logs -n 100 --tail
```

## Producción 

```
https://imageniacellphone.herokuapp.com/
```