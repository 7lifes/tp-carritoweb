# tp-inventario
# nombre de grupo: iroman
## Integrante
- Daniel Paucar
# UP inventario de productos
Proyecto para la materia Arquitectura Web - UP

## Temática de la aplicación

manejo de los productos de un almacen

## Descripción de la aplicación

La aplicación permitirá:

- Administrar un producto (alta, baja, modificacion, listado)
- Administrar un conjunto de productos (alta, baja, modificacion, listado)
- Agrupar productos
- Ordenar productos en orden ascendente y descendente
- Ordenar los grupos de producto en orden ascendente y descendente

Atributos:

- Atributos de un producto:
  - ID
  - descripcion
  - tipo de producto
  - stock
  - precio
  - vencimiento
  - peso
  

- Atributos de un grupo de productos:
  - ID
  - Nombre
  - productos

## API REST

### Endpoints

URL                             | Verbo HTTP  | Resultado
 
/productos                      | GET        | Retorna todos los productos
/productos                      | POST       | Crea un producto
/productos/:id                   | GET        | Retorna un producto determinado
/productos/:id                   | PUT        | Actualiza un producto determinado
/productos/:id                   | DELETE     | Elimina un producto determinado
/productos?sort=az\|za           | GET        | Retorna todos los productos, ordenados en forma ascendente o descendente (A-Z o Z-A)
/productGroups                  | GET         | Retorna todos los grupos de productos
/productGroups                  | POST       | Crea un grupo de productos
/productGroups /:id              | GET    | Retorna un grupo de producto determinado
/productGroups /:id              | PUT   | Actualiza un grupo de productos determinado
/productGroups /:id           | DELETE  | Elimina un grupo de productos determinado
/productGroups ?sort=az\|za   | GET     | Retorna todos los grupos de productos, ordenados en forma ascendente o descendente (A-Z o Z-A)
/productGroups /:id/productos    | GET     | Retorna los productos de un grupo determinado
