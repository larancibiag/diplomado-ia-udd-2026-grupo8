# Tutorial rápido de GitHub

**Diplomado IA Aplicada al Diseño · UDD**

Guía breve para entender lo básico de GitHub: crear un repositorio, entender su estructura (main, branch, tag), y las herramientas sociales de la plataforma (pin, watch, fork, star).

---

## 1. Crear un repositorio

Un repositorio (o "repo") es la carpeta de un proyecto, con todo su historial de cambios incluido.

1. Entra a [github.com](https://github.com) con tu cuenta.
2. Arriba a la derecha, click en el ícono **+** → **New repository**.
3. Ponle un nombre (sin espacios, usa guiones: `mi-proyecto-ia`).
4. Elige si va a ser **Public** (cualquiera lo ve) o **Private** (solo tú y quienes invites).
5. Marca la casilla **Add a README file** — así parte con un archivo de descripción.
6. Click en **Create repository**.

Listo, ya tienes tu repositorio.

---

## 2. Main

`main` es la **rama principal** del repositorio — la versión "oficial" y estable del proyecto. Es la que se crea automáticamente al hacer el repositorio, y en general es la que se muestra por defecto cuando alguien entra a verlo.

Antes se llamaba `master`; GitHub cambió el nombre por defecto a `main` hace unos años.

---

## 3. Branch (rama)

Una **branch** es una copia paralela del proyecto donde puedes trabajar sin afectar `main`. Sirve para probar cosas, agregar una función nueva o corregir un error, sin arriesgar la versión estable.

Cuando terminas y estás conforme con los cambios, puedes fusionar (*merge*) esa rama de vuelta a `main`.

Ejemplo de flujo típico:

```
main
 └── branch: nueva-clase-embeddings   (trabajas acá tranquilo)
       └── cuando está listo → merge a main
```

---

## 4. Tag (etiqueta)

Un **tag** marca un punto exacto en la historia del proyecto — normalmente para señalar una versión (`v1.0`, `v2.0-final`). A diferencia de una branch, un tag no se mueve ni sigue creciendo: es como una foto fija de cómo estaba el repo en ese momento.

Se usa cuando quieres poder volver después a "la versión que entregué el 15 de agosto", por ejemplo.

---

## 5. Pin (fijar)

Sirve para **destacar repositorios en tu perfil** de GitHub, para que sean lo primero que la gente ve cuando entra a tu página. Útil para mostrar tu portafolio o los proyectos del diplomado que quieras exhibir.

También puedes fijar (*pin*) issues o comentarios dentro de un repositorio, para que queden siempre visibles arriba.

---

## 6. Watch (observar)

Al darle **watch** a un repositorio, te llegan notificaciones cada vez que hay actividad ahí: nuevos commits, issues, pull requests, etc. Es útil para seguir de cerca un proyecto sin tener que revisarlo manualmente todos los días.

---

## 7. Fork (bifurcar)

Un **fork** crea una copia completa de un repositorio ajeno dentro de tu propia cuenta. Puedes modificarla libremente sin afectar el original — es la forma estándar de proponer cambios a un proyecto de otra persona, o de tomar un proyecto existente como base para el tuyo.

Después de hacer cambios en tu fork, puedes proponer que se incorporen al proyecto original mediante un **pull request**.

---

## 8. Star (estrella)

Es literalmente un "me gusta": marca un repositorio como favorito. Sirve para guardarlo y encontrarlo fácil después, y también funciona como medida social de qué tan popular o útil es un proyecto (cuántas estrellas tiene).

---

## 9. ¿Puedo crear una carpeta o mover un archivo?

**Sí, ambas cosas se pueden**, aunque GitHub no tiene un botón literal de "nueva carpeta" en la interfaz web — hay que hacer un pequeño truco:

**Crear una carpeta (desde el navegador):**
Ve a **Add file → Create new file**, y en el nombre del archivo escribe la ruta completa incluyendo la carpeta, por ejemplo `notebooks/clase_24.ipynb`. GitHub crea automáticamente la carpeta `notebooks/` al guardar.

**Mover o renombrar un archivo (desde el navegador):**
Entra al archivo → ícono de lápiz (editar) → cambia el nombre en el campo de arriba, agregando la carpeta si quieres moverlo (ej: de `clase_24.ipynb` a `notebooks/clase_24.ipynb`) → **Commit changes**.

**Si trabajas desde tu computador con Git instalado:**

```bash
mkdir notebooks
git mv clase_24.ipynb notebooks/clase_24.ipynb
git commit -m "Organizar notebooks en carpeta"
git push
```

---

## Resumen en una tabla

| Término | Para qué sirve |
|---|---|
| **main** | Rama principal, la versión oficial del proyecto |
| **branch** | Copia paralela para trabajar sin romper `main` |
| **tag** | Marca fija de una versión específica del historial |
| **pin** | Destacar un repo (o issue) para que se vea primero |
| **watch** | Recibir notificaciones de actividad en el repo |
| **fork** | Copiar un repo ajeno a tu cuenta para modificarlo |
| **star** | Marcar un repo como favorito / mostrar apoyo |
