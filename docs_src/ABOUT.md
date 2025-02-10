# Guía de Instalación y Ejecución

Este documento describe los pasos necesarios para instalar y ejecutar la aplicación en tu sistema, ya sea Windows o Linux.

## Requisitos Previos

Asegúrate de tener lo siguiente instalado en tu sistema antes de comenzar:
- Python 3.x
- pip (gestor de paquetes de Python)

## Pasos de Instalación y Ejecución

### 1. Instalación de Python 3

#### En Windows:
1. Descarga el instalador de Python desde [python.org](https://www.python.org/downloads/).
2. Durante la instalación, asegúrate de marcar la opción **"Add Python to PATH"** antes de hacer clic en "Install Now".
3. Verifica la instalación abriendo una terminal (CMD) y ejecutando el siguiente comando:
    ```bash
    python --version
    ```

#### En Linux:
1. En la mayoría de las distribuciones de Linux, Python 3 viene preinstalado. Si no está instalado, puedes instalarlo usando el gestor de paquetes de tu distribución.

    Para **Ubuntu/Debian**:
    ```bash
    sudo apt update
    sudo apt install python3
    ```

    Para **Fedora/RHEL**:
    ```bash
    sudo dnf install python3
    ```

2. Verifica la instalación ejecutando:
    ```bash
    python3 --version
    ```

### 2. Instalación y Activación de pip

#### En Windows y Linux:
1. **pip** suele instalarse junto con Python. Si no está instalado, puedes instalarlo ejecutando:
    ```bash
    python -m ensurepip --upgrade
    ```

2. Verifica la instalación de pip ejecutando:
    ```bash
    pip --version
    ```

### 3. Creación y Activación de Entorno Virtual

#### En Windows:
1. Abre una terminal y navega a la carpeta de tu proyecto.
2. Crea un entorno virtual con el siguiente comando:
    ```bash
    python -m venv venv
    ```
3. Activa el entorno virtual:
    ```bash
    .\venv\Scripts\activate
    ```

#### En Linux:
1. Abre una terminal y navega a la carpeta de tu proyecto.
2. Crea un entorno virtual con:
    ```bash
    python3 -m venv venv
    ```
3. Activa el entorno virtual:
    ```bash
    source venv/bin/activate
    ```

### 4. Instalación de Dependencias

Con el entorno virtual activado, instala las dependencias del proyecto ejecutando:
```bash
pip install -r requirements.txt
