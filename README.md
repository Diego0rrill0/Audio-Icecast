# Proyecto de Servidores de Audio 

Este repositorio contiene los ejercicios realizados para configurar servidores de distribución de audio en Linux y Windows, reconocer y utilizar formatos de audio digital, implementar canales RSS para sindicación y suscripción de audio, y describir un servicio de audio para la empresa ficticia GreyCloud.

## Comenzando 🚀

Estas instrucciones te permitirán obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas.

Mira **Deployment** para conocer cómo desplegar el proyecto.

### Pre-requisitos 📋

- Tener configurados servidores Icecast en Linux Server (Ubuntu) y Windows Server.
- Tener un cliente de audio (VLC) en los sistemas operativos para pruebas.

### Instalación 🔧

1. **Instalar Icecast en Linux**:
   - Actualiza los repositorios:  
     `sudo apt-get update`
   - Instala Icecast:  
     `sudo apt-get install icecast2`
   - Configura Icecast editando el archivo de configuración en `/etc/icecast2/icecast.xml`.

2. **Instalar Icecast en Windows**:
   - Descarga Icecast desde [aquí](https://icecast.org/download).
   - Configura el archivo de configuración de Icecast en `C:\Program Files\Icecast\config\icecast.xml`.

3. **Reproductores de Audio**:
   - Instalar VLC en Windows y Linux para reproducir los audios desde los servidores.

## Ejecutando las pruebas ⚙️

### Análisis de Formatos de Audio Digital 🔩

- Se analizaron los siguientes formatos de audio:
  - **MP3**: Alta compatibilidad y compresión con pérdida.
  - **AAC**: Mejor calidad a tasas de bits similares a MP3.
  - **OGG Vorbis**: Código abierto y de buena calidad.
  - **FLAC**: Calidad sin pérdida de compresión.

- Los archivos de audio fueron reproducidos en el cliente usando VLC y verificados en el servidor Icecast.

### Pruebas de Sindicación con RSS ⌨️

- Se creó un archivo `feed.rss` para permitir la suscripción de los usuarios al contenido de audio.
- El archivo RSS fue probado usando **Akregator** en un cliente Linux, lo que permitió verificar que la sindicación y suscripción funcionaban correctamente.

## Despliegue 📦

Para implementar el servicio de audio, sigue los pasos detallados en **Instalación** para configurar el servidor Icecast en las plataformas Linux y Windows. Una vez configurado, podrás acceder al contenido de audio en tiempo real o bajo demanda.

## Construido con 🛠️

- **Icecast**: Servidor de distribución de audio.
- **VLC Media Player**: Herramienta de reproducción de audio.
- **XML**: Para la creación de canales RSS.


## Autores ✒️

- **Diego Orrillo** - *Trabajo Inicial* - [Diego0rrill0](https://github.com/Diego0rrill0)

---

## Ejercicios

### Ejercicio 1: Implementación de Servidores de Audio

**Objetivo:** Implementar servidores Icecast en Linux y Windows para la distribución de audio en tiempo real.

**Desarrollo Linux:**
- Instalación y configuración de Icecast2 en Ubuntu Desktop.
- Configuración del archivo `icecast.xml` (incluyendo IP, autenticación, etc.).
- Acceso al servidor desde el navegador:  
  `http://192.168.1.95:8000/`
- Confirmación de funcionamiento al acceder al panel de administración.

**Desarrollo Windows:**
- Instalación de Icecast en Windows Server.
- Configuración de la misma forma que en Linux.
- Ejecución del servidor en Windows.

**Conclusiones:**
- Implementación exitosa del servidor Icecast en dos plataformas.
- Comprensión de la configuración y la importancia de los ajustes de red.

---

### Ejercicio 2: Análisis de Formatos de Audio Digital

**Objetivo:** Reconocer y analizar los formatos de audio más populares y probar su compatibilidad con el servidor Icecast.

**Desarrollo:**
- Investigación sobre los formatos MP3, AAC, OGG Vorbis y FLAC.
- Reproducción de los archivos en VLC.
- Inserción de los archivos en el servidor Icecast, superando un problema con las rutas de acceso a los archivos.

**Conclusiones:**
- Se comprobaron la calidad y compatibilidad de los diferentes formatos de audio.
- Todos los formatos funcionaron correctamente después de corregir un problema de configuración en el servidor.

---

### Ejercicio 3: Implementación de Sindicación con RSS

**Objetivo:** Crear un canal RSS para la suscripción de contenido de audio en el servidor Icecast.

**Desarrollo:**
- Creación de un archivo `feed.rss` que contiene información básica del canal y los audios disponibles.
- Pruebas de suscripción usando el cliente **Akregator** en Linux.
- Verificación del funcionamiento del streaming desde el archivo RSS.

**Conclusiones:**
- El sistema de sindicación funcionó correctamente, permitiendo a los usuarios suscribirse a contenido de audio.
- Comprensión de la integración de RSS con servidores de distribución de audio.

---

### Trabajo 2: Funcionalidad del Servicio de Audio

**Objetivo:** Describir cómo el servicio de audio puede ser implementado en una empresa ficticia.

**Desarrollo:**
- La empresa **GreyCloud** se dedica a la ciberseguridad y distribución de software.
- El servicio de audio incluye autenticación, una interfaz amigable, y diversos tipos de contenido para empleados, clientes corporativos y audiencia general.
- Los formatos utilizados son MP3, AAC, FLAC y OGG.

**Conclusiones:**
- El servicio de audio mejora la comunicación interna y ofrece herramientas para clientes.
- El uso de múltiples formatos garantiza flexibilidad y calidad.

---

### Ejercicio 2: Conexión de Clientes al Servidor de Audio

**Objetivo:** Conectar clientes Windows y Linux al servidor de audio para acceder a los archivos.

**Desarrollo:**
- Instalación de VLC en clientes Windows y Linux.
- Conexión al servidor Icecast y verificación del acceso a los archivos de audio.

**Conclusiones:**
- Conexión exitosa desde ambos sistemas operativos, demostrando la funcionalidad multiplataforma del servicio.

---

### Ejercicio 3: Reproducción de Audio desde Clientes

**Objetivo:** Utilizar herramientas de reproducción como VLC para escuchar contenido almacenado en el servidor de audio.

**Desarrollo:**
- Reproducción de contenido desde clientes Windows y Linux utilizando VLC.
- Verificación de la estabilidad del servicio y la calidad de la transmisión.

**Conclusiones:**
- El contenido se reprodujo correctamente desde ambos clientes, lo que confirma la estabilidad y funcionalidad del servicio.
