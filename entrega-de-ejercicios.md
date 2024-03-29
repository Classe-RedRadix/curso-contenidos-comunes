# Entregar los ejercicios de Classe

Los cursos que realizamos en Classe son principalmente prácticos, es como mejor se aprende.

Por ello a lo largo del curso os proponemos realizar varios ejercicios y un ejercicio final que podéis hacer a vuestro ritmo.

## ¿Cómo subir un ejercicio?

Si quieres subir un ejercicio para que el profesor le eche un ojo, para compartirlo con el resto de la clase o para preguntar alguna duda, **lo que tienes que hacer es subir tu ejercicio a una PR desde la rama `promocion-[año]-[mes]-[tu-nombre]` a la rama `promocion-[año]-[mes]`**. A continuación te detallamos cómo:

1. Clona el repositorio del curso.
2. Cámbiate a la rama del curso, que se llamará algo como `promocion-[año]-[mes]`.
3. Crea **una nueva rama a partir de la rama del curso**, una rama para ti. El nombre será igual que la rama del curso pero con tu nombre a continuación: `promocion-[año]-[mes]-[tu-nombre]`.
   ```bash
   # Por ejemplo, para alguien llamada Inés
   git switch promocion-2023-febrero # Me muevo a la rama del curso.
   git switch -c promocion-2023-febrero-ines # Creo la rama y y me muevo a ella.
   ```
   > Recuerda actualizar la rama personal, con la rama del curso. Esto se puede hacer antes o después del commit. Ver el punto [**Actualizar nuestra rama personal, con la rama del curso**](#actualizar-nuestra-rama-personal-con-la-rama-del-curso) para más información.
4. Edita el archivo del ejercicio solicitado, o si no existe este archivo, **crea uno donde implementar el código de la solución del ejercicio**.
5. Añade ese archivo a staging y **crea un commit con un mensaje descriptivo de lo que hemos hecho**, y súbelo a tu rama.
   ```bash
   git add . # Añade todas las modificaciones a staging
   git commit -m "Finished exercise-III, module 2" # Añade un mensaje descriptivo
   git push origin promocion-2023-febrero-ines
   ```
6. [Crea una Pull Request](https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) para que el profesor revise el cambio y lo añada a la rama del curso. **Tenemos que copiar el enlace de esa PR y añadirlo al canal de slack del curso**. Esta Pull Request siempre será usando **la rama del curso como base**.

## Actualizar mi rama personal con la rama del curso

Para poder añadir los cambios a la rama del curso, recomendamos actualizar antes de subir los cambios, con la rama del curso. Esto hará que cualquier cambio posterior que se realice no suponga un conflicto.

Ejemplos:

```bash
# Estando en nuestra rama:

git switch promocion-2023-febrero # Me cambio a la rama del curso
git pull origin promocion-2023-febrero # Me traigo los cambios de esta rama
git switch promocion-2023-febrero-ines # Me cambio a mi rama otra vez
git merge promocion-2023-febrero # Mergeo la rama promocion-2023-febrero-ines en promocion-2023-febrero
```

[Más información sobre git merge.](https://www.freecodecamp.org/espanol/news/la-guia-definitiva-para-git-merge-y-git-rebase/)

## Documentación de ayuda

- [git switch](https://git-scm.com/docs/git-switch)
- [git add](https://git-scm.com/docs/git-add)
- [git commit](https://git-scm.com/docs/git-commit)
- [git push](https://git-scm.com/docs/git-push)
