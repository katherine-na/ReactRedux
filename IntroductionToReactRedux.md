<h1 align="center"> Redux </h1>

## Getting Started with Redux

Redux es una biblioteca de JavaScript para administrar el estado de la aplicación.

<img src="https://redux.js.org/assets/images/one-way-data-flow-04fe46332c1ccb3497ecb04b94e55b97.png" />

### State Management
- **State**  
  Permite que la vista se renderice.
- **View**  
  A través de una acción (event, click, etc) => Desencadena una acción.
- **Actions**  
  Cambian el estado.

El estado se actualiza => El estado se comunica con la vista => La vista pinta el estado

## Actions
Una acción es un objeto JavaScript simple que se compone de dos keys con valores.

- **Type:** ¿Qué tipo de comportamiento quiero desencadenar con esta acción?
El type siempre sera un string a través del cual tu dices: Quiero agregar, quiero eliminar, quiero actualizar, etc.
- **Payload:**  Es la información que quieres enviar al state para que se actualice 

## Reducer 
Un reducer es una función que toma dos argumentos.
El argumento inicial sera el **state** y el segundo sera el **action** 
Esta función se encargara de actualizar el **state** 
Toma el **state** previo, toma el **action** (que viene con el type y el payload) y de esa manera va a generar la actualización del estado

## Store
El store es el lugar donde se almacena todo el estado de la aplicación. El store es la unión de todos los reducers.

## Dispatch 
El dispatch es una función que lo que hace es disparar los actions creator para que ejecute el reducer y sepa que hacer  

<img src="https://redux.js.org/assets/images/ReduxDataFlowDiagram-49fa8c3968371d9ef6f2a1486bd40a26.gif" />
