# Instalación del Compilador `gcc` en Mac

En Mac una opción sencilla es utilizar el [gestor de paquetes Homebrew](https://brew.sh/). A continuación, se explican los pasos de manera general. Es importante tener en cuenta que todos los comandos se tienen que ejecutar desde [la terminal de comandos de Mac](https://support.apple.com/es-es/guide/terminal/apd5265185d-f365-44cb-8b09-71a064a42125/mac).

1. Instalar los [Command Line Tools de Apple](https://developer.apple.com/la/documentation/xcode/installing-the-command-line-tools) ejecutando el siguiente comando en la terminal (la ejecución puede tardar hasta media hora, así que hay que ser paciente).

    ```shell
    xcode-select --install
    ```

2. Una vez que se instalan las command lines tools, instalar el gestor de paquetes ejecutando desde el terminal, el siguiente comando:

    ```shell
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

3. Una vez instalado Homebrew, el compilador `gcc` de instala ejecutando el siguiente comando desde el termina:

    ```shell
    brew install gcc
    ```

Para asegurarse de que el compilador se ha instalado, ejecutar el siguiente commando:

```shell
gcc --version
```
