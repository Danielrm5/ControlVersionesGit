# 5.- Conceptos básicos Git/GitHub

Para trabajar fluidamente en entornos profesionales, es imperativo dominar el vocabulario y la mecánica de estas herramientas:

* **Repositorio (Repo):** Es el contenedor principal de un proyecto. Técnicamente es un directorio donde Git ha sido inicializado (creando una carpeta oculta `.git` que contiene todo el historial). Puede existir localmente en tu ordenador o remotamente en servidores como GitHub.
* **Clone (Clonar):** El comando `git clone` descarga un repositorio remoto completo (todo el código, todas las ramas y todo el historial de commits) a tu máquina local para que puedas trabajar en él.
* **Fork (Bifurcación):** Es un concepto exclusivo de plataformas como GitHub (no de Git puro). Consiste en hacer una copia exacta del repositorio de otra persona en tu propia cuenta de GitHub. Esto te da permisos de escritura totales sobre tu copia sin afectar al proyecto original.
* **Commit:** Es la unidad básica de guardado en Git. No es simplemente un "guardar"; es una captura o instantánea del estado de todos los archivos en ese milisegundo exacto. Cada commit genera un código hash único (SHA-1) que lo identifica, está asociado a un autor, una fecha y un mensaje obligatorio que explica *qué* se cambió y *por qué*.
* **Rama (Branch):** Es un puntero móvil que apunta a un commit específico. La rama principal y por defecto suele llamarse `main` o `master`. Crear ramas permite a los desarrolladores bifurcar el código para trabajar en nuevas características (features) o arreglar bugs de forma aislada, sin inestabilizar el código principal en producción.
* **Push:** El comando `git push` sube tus commits locales (que solo existen en tu disco duro) al repositorio remoto, sincronizando los cambios para que el resto del equipo pueda verlos.
* **Pull:** El comando `git pull` hace lo contrario; descarga los últimos cambios realizados por otros miembros del equipo desde el repositorio remoto y los fusiona automáticamente con tu entorno de trabajo local.
* **Merge (Fusión):** Es el proceso de unir dos historias de desarrollo (dos ramas) en una sola. Si tú estabas trabajando en una rama "desarrollo" y terminas tu trabajo, haces un merge para volcar todo ese código en la rama "main". Si otros modificaron las mismas líneas de código que tú al mismo tiempo, Git reportará un **Conflicto**, que deberá resolverse manualmente.
* **Pull Request (PR) / Merge Request:** Es un mecanismo web (en GitHub, GitLab, etc.) donde avisas al equipo de que has terminado una tarea en tu rama. El PR abre un espacio de discusión donde otros desarrolladores pueden revisar tu código línea por línea, sugerir cambios, aprobarlos y, finalmente, hacer clic en un botón para ejecutar el Merge en el proyecto principal de forma segura.

<img src="img/conceptos.png" alt="Conceptos de Git" width="400" height="250"/>
