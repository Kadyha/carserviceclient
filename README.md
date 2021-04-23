# CarServiceClient

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.1.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).


# Explicación sobre los componentes y serviscios realizados en angular para llegar a la solución.

## carOwner-list (componente)

Presenta una lista de carros con sus propietarios, los carros presentan una imagen de estos. Este componente funciona igual que car-list, pero se agrego el nombre del propietario para que este sea listado junto al nombre del auto, el nombre del propietario es guardado en el parametro car.ownerDni.

## car-edit (componente)

Este componente fue modificado para permitir agregar el propietario. Para lograrlose modifico el componente shared, y dentro de este el llamado car, este componente paso a llamarse carOwner, y fue modificado para funcionar también con la API de owners y de esta forma ambas API fueron usadas como un mismo servicio.

## Owner-list (componente)

Permite ver una lista de propietarios. Este componente funciona igual que car-list, pero se lista unicamente el parametro car.ownerDni ya que este contiene el nombre del usuario, además, cada uno tiene un botón que permite eliminarlo, esto elimina tanto los datos del auto como los datos del propietario, de esta forma se puede usar la lista para eliminar varios propietarios al tiempo.

## Owner-edit (componente)

Permite crear y actualizar propietarios. Para lograrlo se uso como base el componente car-edit, y de igual forma se usaron los servicios de ambas API, para relacionarlas entre sí al crear un nuevo prietario.
