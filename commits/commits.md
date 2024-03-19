# ¿Cómo hacer un buen Commit en Git?
Para poder crear un commit utilizaremos el commando git commit

```bash
git commit -m "feat(users): enable user profile"
```

El flag -m agregado al comando git commit nos permitirá agregar un commit a la rama que estamos trabajando y de nueva cuenta aquí vuelve a existir otro conflicto, ya que si no tenemos estructuras, estándares o referencias para poder generarlos, seguramente se volverán un caos.

Ten en consideración lo siguiente: Probablemente el commit que generas hoy, lo tendrás que volver a revisar en algún tiempo: días, semanas, meses o años y si no damos la descripción adecuada, probablemente se vuelva un lío.

Para que esto no suceda, en la comunidad hay distintas sugerencias, sin embargo, una de las más utilizadas, se denomina conventional commits.

En términos resumidos, conventional commits sugiere lo siguiente:

### El mensaje del commit deberá seguir una estructura, la cual es:

```
<tipo>[ámbito opcional]: <descripción>

[cuerpo opcional]

[nota(s) al pie opcional(es)]
```
Por lo que las recomendaciones son:

**El commit siempre deberá iniciar con un tipo**, algunos de los tipos disponibles que comúnmente se pueden agregar son:

- **feat:** Agregar nueva funcionalidad.
- **fix:** Al arregla un error.
- **chore:** Tareas que no sean una nueva funcionalidad como:
  - crear un gitignore
  - actualizar el readme file
  - agregar nueva librería o dependencia
- **test:** Agregar o modificar tests.
- **docs:** Agregar o modificar documentación.
- **refactor:** Refactorizar el código.
- **perf:** Mejorando el rendimiento o performance

Lo siguiente es que el ámbito puede ser opcional, como lo menciona la estructura, por ejemplo: podemos poner api, que significa que el ámbito es la api, o user, que significaría el módulo de usuarios, etc.

[Buenas prácticas para escribir commits en Git](https://midu.dev/buenas-practicas-escribir-commits-git/)

**Se deberá agregar la descripción de commit, empezando siempre por un verbo en imperativo**, por ejemplo:

añade, crea, remueve, cambia, soluciona y la descripción que generemos.

(Add, Change, Fix, Remove, …)


> [!IMPORTANT]
> NO se usan puntos finales al término de la descripción y La séptima recomendación es: La descripción deberá tener como máximo hasta 50 caracteres.

A continuación te recomiendo ver lo siguiente: [Como crear una pull request con buenas prácticas](/pull_request/pull_request.md)
