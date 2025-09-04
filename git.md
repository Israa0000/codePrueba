# GIT
## Instalaciones

Para poder utilizar git en nuestro entorno se tendra que instalar dicha aplicacion, pero aparte instalaremos gitHub cli, para poder para poder crear un repositorio desde la terminal (aparte de mas funciones pero esta sera la principal)

### Instalar git 
- Windows 
    - descargaremos el ejecutable desde https://git-scm.com/downloads/win y lo instalaremos


- Linux 
    - $ apt-get install git

### Instalar GitHub Cli

- Windows 
    - descargaremos el ejecutable desde https://cli.github.com/
    - o utilizaremos `winget install --id GitHub.cli` en la terminal y despues lo actualizaremos con `winget upgrade --id GitHub.cli`

    - para confirmar que se ha instalado correctamente meteremos `gh --version`, si no hay ningun problema aparecera en este formato `gh version 2.x.x (2025-xx-xx)`

    - en caso de que nos aparezca `gh : El término 'gh' no se reconoce como nombre de un cmdlet, función, archivo de script o programa ejecutable` o un mensaje parecido quiere decir que no se encuentra el ejecutable en la variable de entorno PATH, para cambiar esto debemos

    1. Verificar que esta instalado:
    Debemos de ir a la dirección `C:\Program Files\GitHub CLI\` y verificar que hay un ejecutable llamado `gh.exe`

    2. Pulsar **Win + R**, escribir `sysdm.cpl` y darle a **Enter**.

    3. **Opciones Avanzadas** -> **Varibles de entrono**

    4. **Varibles del sistema**, buscar **PATH** y pulsar **editar**

    5. Añadir la ruta a donde se encuantra el ejecutable por ejemplo
        `C:\Program Files\GitHub CLI\`

    6. Guarda y cierra

    7. Abre una nueva terminal e introduce el comando `gh --version`
    y la deberia demostrar algo tal que asi `gh version 2.x.x (2025-xx-xx)`


- Linux 
    - `sudo apt install gh`
    - `sudo apt update gh` para actualizar


### Configuración 

- GitHub Cli

    Necesitaremos acceder a nuestra cuenta para poder crear los repositorios utilizaremos `gh auth login` y nos dira lo siguiente
    - `? Where do you use GitHub?` selecionamos `GitHub.com`
    - `? What is your preferred protocol for Git operations on this host?` seleccionamos la opcion que se adapte a nosotros
    - La siguiente linea varia depende de la anterior en caso de que nos diga `? Generate a new SSH key to add to your GitHub account?` o algo parecido elejimos `no`
    - `? How would you like to authenticate GitHub CLI?` elejimos `Login with a web browser` hecho esto nos dara un codigo
    Nos loguemos en la pagina y tendremos que meter el codigo
    - Hecho esto ya hemos terminado

 
### Creacion del repositorio

Como crear un repositorio desde cero 
`gh repo create`

`Create a new repository on github.com from scratch` en esta ocasion elegiremos esta opción

`Repository name` Escogemos el nombre del repositorio

`Description` Añadimos una descripción (se puede saltar)

`Visibility` Elegimos la visibilidad del repositorio entre `Public` o `Private`

`Would you like to add a README file? (y/N)` elegimos si queremos añadir un README

`Would you like to add a .gitignore? (y/N)` elegimos si queremos añadir un .gitignore

`Would you like to add a license? (y/N)` elegimos si queremos añadir una licencia

`This will create "Name" as a "Visibility" repository on github.com. Continue? (Y/n)` Le damos a si

`Clone the new repository locally? (y/N)` Clonar el repository a nuestro dispositivo (en la direccion actual) esto es a eleccion 

**Ya tendriamos nuestro repositorio creado**

### Guardar progreso en nuestro repositorio
Una vez creado nuestro repositorio podemos guardar todo el codigo y añadir una pequeña descripcion de cada movimiento 

El proceso se empieza de esta manera
