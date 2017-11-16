# README #

## Componente tabla-árbol (tabletree) ##

* [Introducción](#introduccion)
* [Versión](#version)
* [¿Cómo me lo puedo instalar?](#install)

<a name="introduccion"></a>
### Introducción: 

Componente tabla árbol simple para proyectos en AngularJS. 


<a name="version"></a>
### Versión 
Versión 3.05: Actualiza el README.md y la versión en el bower.json

<a id="install"></a>
### __¿Cómo me lo puedo installar?__

* [Instalación](#download)
* [¿Cómo lo Uso?](#uso)

<a id="download"></a>
### Descarga e instalación:

`bower install -S https://github.com/krbaio3/atmira-tabletree.git`

<a id="uso"></a>
#### __¿Cómo lo Uso?:__

Inyectar la dependencia en el módulo AngularJS:

```javascript
  angular.module('nombre.ejemplo',['atmira.ui.tabletree']);
```

En la vista (html) donde se vaya a usar aplicar la directiva ``atmira-ui-tabletree``:

```html
    <atmira-ui-tabletree tree-data="nombreControlador.tree_data"></atmira-ui-tabletree>
    <atmira-ui-tabletree tree-data="nombreControlador.arrayAmostrar" 
                         col-defs="nombreControlador.dealFundsDesTree_defs" 
                         expand-on="nombreControlador.dealFundsDesTree_expand" 
                         template-url="app/components/newDeal.module/modal.component/runDeal/tableTreeTemplate.html">
    </atmira-ui-tabletree>
```
Inyectar el JS y el CSS en el index.html del proyecto:

  ```html

    <link rel="stylesheet" href="./bower_components/atmira-ui-tabletree/dist/tabletree.css">

    <script src="./bower_components/atmira-ui-tabletree/dist/tabletree.js"></script>

  ```  

En el controlador de la vista donde se vaya a usar crea un array:

```javascript
     vm.tree_data = [{ Name:"USA",Area:9826675,Population:318212000,TimeZone:"UTC -5 to -10",
          children:[
                    {
                      Name:"California", Area:423970,Population:38340000,TimeZone:"Pacific Time"
                    },
                    {
                      Name:"Illinois", Area:57914,Population:12882135,TimeZone:"Central Time Zone"
                    }
                  ]
      },
      {
          Name:"Texas",Area:268581,Population:26448193,TimeZone:"Mountain",
          children:[
            {
              Name:"Illinois", Area:57914,Population:12882135,TimeZone:"Central Time Zone"
              }
          ]
      }];
```
