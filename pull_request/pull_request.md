# Mejores prácticas Pull Request

> [!TIP]
> Los Pull Request deben ser pequeños con el objetivo de tomarle la seriedad necesaria al Code Review,

La revisión del código es una parte muy importante del ciclo de desarrollo de software. Las solicitudes de extracción se utilizan para revisar el código en las ramas antes de que llegue al maestro. La revisión del código es también una de las partes más difíciles y que consumen más tiempo del proceso de desarrollo de software, y a menudo requiere que miembros del equipo experimentados dediquen tiempo a leer, pensar, evaluar y responder a implementaciones de nuevas funciones o sistemas.

## General

Cuanto más pequeñas sean las Pull Requests, mejor.

### Escribe una buena descripción

Escribir una buena descripción en una Pull Request es una de las partes más importantes y que más ayudarán a la hora de revisarla. Si la persona que revisa el código ve 300 líneas añadidas, 100 borradas y varios archivos renombrados, lo más probable es que no sepa el motivo de esos cambios, así que para ayudarle a revisar tu código, deja una buena descripción en la que expliques qué has hecho y por qué.

Escribir una descripción completa en una Pull Request ayudará a dar contexto en la revisión.

[Usar un Template para PR's](/doc/PULL_REQUEST_TEMPLATE/pull_request_template.md)

### Para el tempate en github

```bash
# root-project
|-- /.github
|   |-- /PULL_REQUEST_TEMPLATE
|   |   |-- pull_request_template.md
```

## Extras
[Sintaxis básica de escritura y formato.
](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#referencing-issues-and-pull-requests)


### ¿Qué se debería automatizar en una Pull Request?

- **Testing:** cada vez que se abre una Pull Request se deberían pasar los tests automáticamente, y también cuando se hace un nuevo commit a una Pull Request ya abierta. A menos que pasen los tests, la rama no se podrá mergear.
- **Documentación:** mantener la documentación es un proceso realmente tedioso, por lo que cuanto más automatizado esté el proceso, mejor. Por ejemplo, si estamos desarrollando una API que tiene documentación podríamos automatizar su generación.

### Responde rápido a los comentarios

Cuando abres una Pull Requests los revisores estarán haciendo un gran esfuerzo por meterse tu problema en la cabeza, y es menos costoso para ellos cambiar de foco varias veces en poco tiempo que en mucho tiempo.

Por ejemplo, si abres una Pull Request y te dejan comentarios, no contestes a los comentarios al día siguiente o a los dos días porque los revisores ya se habrán olvidado de ella y necesitarán un buen rato para volver a ponerse en contexto. Sin embargo, si la cerráis en 3 horas ya tendrán el problema en la cabeza y les costará menos cambiar su foco de concentración.