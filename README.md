# Ramificación Inteligente

### 1. Rama de producción (master)
Esta rama representa la última base de código lanzado/implementado. Sólo es actualizada mediante la fusión de otras ramas en él.
### 2. Rama de desarrollo (develop)
Esta es la rama de desarrollo principal, donde se colocan todos los cambios destinados a la próxima versión, ya sea mediante la confirmación directa de pequeños cambios o mediante la fusión de otras ramas (por ejemplo, ramas de características) en esta rama.
### 3. Ramas de características (feature/) 
```git
git checkout -b feature/[name_branch] 
```
Cuando comienza a trabajar en algo no trivial, crea una rama de características. Cuando termine, volverá a combinar esta rama en la rama de desarrollo para ponerla en cola para la próxima versión.
### 4. Ramas de lanzamiento (release/) 
Cuando está a punto de empaquetar un nuevo lanzamiento, crea una rama de lanzamiento desde la rama de desarrollo. Puede comprometerse con él durante su preparación para un lanzamiento, y cuando esté listo para ser implementado, lo fusiona tanto en la rama de desarrollo como en la rama maestra (para indicar que el lanzamiento se ha implementado).
### 5. Sucursales de revisión (hotfix/) 
Si necesita parchear la última versión sin recoger las nuevas características de la rama de desarrollo, puede crear una sucursal de revisión del último código implementado en el maestro. Una vez que haya realizado los cambios, la rama de hotfix se fusionará nuevamente con la rama maestra (para actualizar la versión publicada) y la rama de desarrollo (para asegurarse de que las correcciones también se incluyan en la próxima versión)
