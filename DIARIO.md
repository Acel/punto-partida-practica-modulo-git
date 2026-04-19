### Tarea 1:

Un fork es copiar el repositorio de otra persona en tu cuenta de github. Al estar en tu propia cuenta, dispones de total libertad para modificar lo que quieras sin afectar al original.

Una vez hecho esto, es habitual necesitar mantener un vínculo con el repositorio original, bien para actualizar mi repositorio local con las últimas novedades, o bien para subir mis cambios al repositorio original mediante un pull request. En definitiva, sincronizarlo con el original. A esto se le llama hacer un remote. Y por convención, en git, a ese vínculo con el repositorio original se le llama upstream.

<img width="852" height="143" alt="image" src="https://github.com/user-attachments/assets/a0a00abf-92bd-4b77-85de-ab3d119ee5ec" />
<img width="1160" height="697" alt="image" src="https://github.com/user-attachments/assets/d3bee5b8-b5bd-487b-9cb8-e6b44d5dea31" />

### Tarea 2:

Nuestra nueva feature partirá de dev y no de main porque dev es nuestra rama de desarrollo y main la de producción. En dev es donde se hacen las pruebas. No tendría sentido desarrollar en main directamente por el rieesgo de errores y de romper cosas en producción sin que estén 100% probadas. Por tanto, el orden lógico es: se crea una rama desde dev, que debe estar lo más actualizada posible con respecto a main. Después se hacen los cambios y pruebas. Cuando nos aseguremos de que nuestra feature funciona como deseamos, se mergea con dev, se pasan tests y se comprueba que dev funciona correctamente. Solo tras todos estos pasos, en algún momento de nuestro ciclo de integración contínua, la rama dev se mergeará en main y pasará a producción.

<img width="1913" height="966" alt="image" src="https://github.com/user-attachments/assets/62b515ac-d752-41e1-8cfd-64c7c76ce276" />

### Tarea 3:

En git se produce un conflicto cuando dos ramas diferentes, que parten de la misma rama original, en nuestro caso dev, hacen modificaciones sobre una misma línea de un mismo fichero, o varios. En este caso, ambas ramas querrán modificar dicha línea de dicho fichero al mergearse con dev. Y aquí es donde surgirá el conflicto: cuál es la información correcta, la de la primera feature o la de la segunda? El usuario en este caso tendrá que decidir manualmente cómo resolver este conflicto. Cuál de las dos versiones elige, o incluso una mezcla de ambas. En nuestro caso concreto el conflicto surgirá en la descripción de la opción 3, que es modificada por ambas features.

### Tarea 4:

En files changed he revisado los cambios de mi rama con respecto a dev. Puedo ver que se ha modificado la descripción de la opción 3 y que se ha añadido la opción 5, tal y como se puede ver en la imagen que se adjunta a continuación. Es recomendable revisar esto para asegurarnos de que realmente se mergea lo correcto, y no cualquier otra cosa por error.

<img width="1917" height="967" alt="image" src="https://github.com/user-attachments/assets/3d06dcdf-9bac-472d-8997-bb1bc34b809e" />

### Tarea 5:

Los marcadores nos sirven para poder diferenciar las dos versiones, es decir, la que tengo en mi rama y la que me viene de dev. El ide me muestra las dos versiones y me pide elegir entre una de las dos, o includo conservar ambas, para poder resolver el conflicto.

<img width="1915" height="970" alt="image" src="https://github.com/user-attachments/assets/6092ccbe-d866-47fb-8016-261b2e5f1ad2" />
<img width="1126" height="641" alt="image" src="https://github.com/user-attachments/assets/6751f156-966e-4cd2-b0d8-0d57cf2bc72d" />
<img width="1915" height="967" alt="image" src="https://github.com/user-attachments/assets/1dfb1439-a5d4-422d-9fe2-b9ecc01f79cc" />

### Tarea 6:

<img width="990" height="272" alt="image" src="https://github.com/user-attachments/assets/c35b63e7-94f4-4267-a029-b9b647f5c2e2" />

Lo más complicado sin duda ha sido el mergeo. Yo además he tenido un conflicto adicional en el mergeo con las opciones 5 y 6, que he tenido que resolver manualmente también. No sé si esto estaba o no planificado en la práctica.
