# Colors API

Mi enfoque en el desarrollo de la aplicación se ha centrado en la modularidad, la escalabilidad y la facilidad de mantenimiento. La arquitectura de la aplicación se ha desglosado en componentes clave, cada uno con roles bien definidos. Aquí se resaltan los aspectos fundamentales de mi enfoque:

Para facilitar una comunicación eficiente entre el servidor y el cliente, he optado por adoptar una arquitectura RESTful. Esto se ha logrado definiendo rutas claras y coherentes que se alinean con los principios fundamentales de la arquitectura REST, lo que en última instancia facilita tanto la comprensión como el mantenimiento del código.

Me he asegurado de establecer una clara separación de responsabilidades al dividir la lógica de la aplicación en capas distintas. Esta separación incluye la disociación de la lógica de enrutamiento, los controladores y la interacción con la base de datos. Este enfoque ha sido fundamental para identificar y corregir errores de manera efectiva en el código.

He implementado pruebas exhaustivas, incluyendo tanto pruebas unitarias como de integración. Este enfoque me ha permitido garantizar la estabilidad y la solidez del código, al tiempo que ha facilitado la identificación temprana de posibles problemas en el comportamiento de la aplicación.

Con el uso de variables de entorno y el módulo dotenv, he gestionado la configuración de manera eficaz. Esto ha posibilitado la configuración sencilla de la aplicación en diversos entornos, lo que ha contribuido a su flexibilidad y adaptabilidad en diferentes contextos.

## Tecnologías Utilizadas

- [Express](https://expressjs.com/) Utilizado como el framework principal para la construcción de la aplicación de backend. Express ofrece una estructura simple y efectiva para manejar solicitudes HTTP y definir rutas.
- [Sequelize](https://sequelize.org/) ORM de Node.js que facilita la interacción con una base de datos relacional, en este caso, MySQL. Permite la definición de modelos de datos y la realización de consultas de manera legible.
- [MySQL2](https://www.npmjs.com/package/mysql2) Controlador MySQL para Node.js, utilizado para establecer la conexión con la base de datos MySQL y realizar operaciones de consulta de manera eficiente.
- [Jest](https://jestjs.io/) Framework de pruebas utilizado para realizar pruebas unitarias exhaustivas en la aplicación. Jest ofrece una amplia gama de funciones para evaluar el comportamiento del código y garantizar su fiabilidad.
- [Supertest](https://www.npmjs.com/package/supertest) Biblioteca de pruebas que simplifica la realización de pruebas de extremo a extremo para la API HTTP de Node.js. Permite la simulación de solicitudes HTTP y la verificación de respuestas.
- [Dotenv](https://www.npmjs.com/package/dotenv)  Módulo para la gestión de variables de entorno. Se utiliza para la carga de variables de entorno desde un archivo .env, lo que garantiza una gestión eficiente de la configuración de la aplicación en diferentes entornos.
- y otras

## Instalación

1. Clona este repositorio.
2. Ejecuta `npm install` para instalar las dependencias.
3. Configura tus variables de entorno en un archivo `.env` en la raíz del proyecto.

## Ejecución del Proyecto

- Ejecuta `npm run dev` para iniciar el servidor en modo de desarrollo.
- Ejecuta `npm run test` para ejecutar las pruebas.

## URL de Producción

_(Opcional)_ Inserta aquí la URL de producción si la aplicación está desplegada.

## Poblar la Base de Datos de Desarrollo

1. Asegúrate de que la base de datos esté configurada correctamente en tu entorno de desarrollo.
2. Ejecuta el siguiente comando para poblar la base de datos con datos de prueba: `npm run db:seed`
Esto generará datos de prueba predeterminados. También puedes especificar la cantidad de datos a generar ingresando un número después del comando, por ejemplo: `npm run db:seed 40`
Esto generará 40 registros en la base de datos.

