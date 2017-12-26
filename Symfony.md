# Bundles

#### Crear un Bundle:
php bin/console generate:bundle --namespace=Acme/TestBundle

# Doctrine:
#### Archivo de Configuracion de la DB
app/config/config.yml

#### Crear una nueva DB
php bin/console doctrine:database:create

#### Eliminar BD
php bin/console doctrine:database:drop --force

#### Generar una nueva Entidad
php bin/console doctrine:generate:entity

#### Generar Getters y Setters de entidades
php bin/console doctrine:generate:entities AppBundle/Entity/Product

#### Crear las tablas
php bin/console doctrine:schema:update --force

### Insertar de fecha de creación desde entity
```php
public function __construct()
{
    $this->createdAt= new \DateTime();
}
```
