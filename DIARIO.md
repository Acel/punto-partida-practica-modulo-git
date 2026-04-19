### Tarea 1:

Un fork es copiar el repositorio de otra persona en tu cuenta de github. Al estar en tu propia cuenta, dispones de total libertad para modificar lo que quieras sin afectar al original.

Una vez hecho esto, es habitual necesitar mantener un vínculo con el repositorio original, bien para actualizar mi repositorio local con las últimas novedades, o bien para subir mis cambios al repositorio original mediante un pull request. En definitiva, sincronizarlo con el original. A esto se le llama hacer un remote. Y por convención, en git, a ese vínculo con el repositorio original se le llama upstream.

<img width="852" height="143" alt="image" src="https://github.com/user-attachments/assets/a0a00abf-92bd-4b77-85de-ab3d119ee5ec" />
<img width="1160" height="697" alt="image" src="https://github.com/user-attachments/assets/d3bee5b8-b5bd-487b-9cb8-e6b44d5dea31" />

### Tarea 2:

Nuestra nueva feature partirá de dev y no de main porque dev es nuestra rama de desarrollo y main la de producción. En dev es donde se hacen las pruebas. No tendría sentido desarrollar en main directamente por el rieesgo de errores y de romper cosas en producción sin que estén 100% probadas. Por tanto, el orden lógico es: se crea una rama desde dev, que debe estar lo más actualizada posible con respecto a main. Después se hacen los cambios y pruebas. Cuando nos aseguremos de que nuestra feature funciona como deseamos, se mergea con dev, se pasan tests y se comprueba que dev funciona correctamente. Solo tras todos estos pasos, en algún momento de nuestro ciclo de integración contínua, la rama dev se mergeará en main y pasará a producción.

<img width="1912" height="963" alt="image" src="https://github.com/user-attachments/assets/5c1fcca6-1ea8-479c-af8f-5a1c3c7d0e02" />

