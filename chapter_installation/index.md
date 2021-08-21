# Instalación
:label:`chap_installation`

Para poder ejecutar el código, necesitaremos un entorno para ejecutar Python, notebooks de Jupiter, las librerías relevantes, y el código necesitado para ejecutar el libro en si mismo.

## Instalando Miniconda

Tu opción más sencilla es instalar
[Miniconda](https://conda.io/en/latest/miniconda.html). 
Notar que la versión 3.x de Python es requisito necesario. 
Puedes saltarte los siguientes pasos si tu máquina ya tiene conda instalado.

Visita la web de Miniconda y determina cual es la versión apropiada para tu sistema
basado en tu versión de Python 3.x y la arquitectura de tu máquina.
Por ejemplo, si tu estás usando macOS y Python 3.x,
tu descargarías el script bash cuyo nombre contiene el texto "Miniconda3" y "MacOSX",
navega a la localización de descarga,
y ejecuta la instalación como sigue:

```bash
sh Miniconda3-latest-MacOSX-x86_64.sh -b
```


Un usuario de Linux con Python 3.x 
descargaría el fichero cuyo nombre contiene el texto "Miniconda3" y "Linux" 
y lo ejecutaría lo siguiente en la localización de descargar:

```bash
sh Miniconda3-latest-Linux-x86_64.sh -b
```


Después, inicializas la shell así puedes ejecutar `conda` directamente.

```bash
~/miniconda3/bin/conda init
```


Ahora cierra y reabre tu actual shell. 
Tu deberías ser capaz de crear un nuevo entorno como sigue:

```bash
conda create --name d2l python=3.8 -y
```


## Descargando los Notebooks de D2L 

Lo siguiente, necesitamos descargar el código de este libro.
Tu puedes pulsar la pestaña "All Notebooks" en la parte de arriba de de cualquier página HTML del libro para descargar y descomprimir el código.
Alternativamente, si tu tienes `unzip` (sino ejecuta `sudo apt install unzip`) disponible:

```bash
mkdir d2l-en && cd d2l-en
curl https://d2l.ai/d2l-en.zip -o d2l-en.zip
unzip d2l-en.zip && rm d2l-en.zip
```


Ahora activamos el entorno `d2l`:

```bash
conda activate d2l
```


## Instalando el Framework y el Paquete `d2l`

Antes de instalar cualquier framework de deep learning,
por favor comprueba si tienes o no una GPU adecuada en tu máquina
(las GPUs que aceleran la pantalla de un portatil standard no son relevantes para nuestros propósitos).
Si estás trabajando en un servidor con GPR, continua con :ref:`subsec_gpu` 
para instrucciones de cómo instalar versiones GPU-compatibles de las librerías relevantes.

Si tu máquina no usa ninguna GPU,
no hay necesidad de preocuparse todavía.
Tu CPU proporciona más que suficiente potencia 
para conseguir que pases por los primeros capítulos.
Sólo recuerda que querrás tener acceso a GPUs
antes de ejecutar modelos más grandes.
Para instalar la versión de CPU,
ejecuta el siguiente comando.


:begin_tab:`mxnet`

```bash
pip install mxnet==1.7.0.post1
```


:end_tab:


:begin_tab:`pytorch`

```bash
pip install torch torchvision
```


:end_tab:

:begin_tab:`tensorflow`
Tu puedes instalar TensorFlow con soporte para ambos CPU y GPU como sigue:

```bash
pip install tensorflow tensorflow-probability
```


:end_tab:


Nuestro siguiente paso es instalar 
el paqeute `d2l` que hemos desarrollado para encapsular
funciones y clases usadas frecuentemente que encontrarás a lo largo de este libro.

```bash
# -U: Upgrade all packages to the newest available version
pip install -U d2l
```


Una vez que tu has completado los pasos de instalación, arrancamos el servidor de notebooks de Jupiter ejecutando:

```bash
jupyter notebook
```


En este punto, tu puedes abrir http://localhost:8888 
(puede que se haya abierto ya automáticamente) en tu navegador.
Entonces nosotros podemos ejecutar el código para cada sección de el libro.
Por favor siempre ejecuta `conda activate d2l` 
para activar el entorno de ejecución
antes de ejecutar el código de el libro
o actualizar el framework de deep learning o el paquete de `d2l`.
Para salir del entorno, ejecuta:run `conda deactivate`.


## Soporte para GPU
:label:`subsec_gpu`

:begin_tab:`mxnet`
Por defecto, MXNet se isntala sin soporte para GPU
para asegurar que se ejecutará en cualquier ordenador (incluyendo la mayoría de los portátiles).
Parte de este libro requiere o recomienda la ejecución con GPU.
Si tu ordenador tiene tarjeta gráfica NVIDIA y tiene isntalado [CUDA](https://developer.nvidia.com/cuda-downloads),
entonces tu deberías instalar la versión con GPU habilitada.
Si tu tienes isntalada la versión de sólo CPU, puede que necesites desinstalarla primero ejecutando

```bash
pip uninstall mxnet
```

Ahora necesitamos encontar que versión de CUDA tienes instalada.
Puedes comprobarlo ejecutando `nvcc --version` 
o `cat /usr/local/cuda/version.txt`.
Asumiento que tienes instalado CUDA 10.1,
entonces puedes instalar con los siguientes comandos:


```bash
# Para usuarios Windows
pip install mxnet-cu101==1.7.0 -f https://dist.mxnet.io/python

# Para usuarios Linux y macOS
pip install mxnet-cu101==1.7.0
```


Puedes cambiar los últimos digitos de acuerdo a tu versión de CUDA, por ejemplo, `cu100` para
CUDA 10.0 y `cu90` para CUDA 9.0.
:end_tab:


:begin_tab:`pytorch,tensorflow`
Por defecto, este framework de deep learning se instala con soporte para GPU.
Si tienes GPUs NVIDIA y has instalado [CUDA](https://developer.nvidia.com/cuda-downloads),
entonces lo tienes configurado.
:end_tab:

## Ejercicios

1. Descarga el código para el libro e instala el entorno de ejecución.

:begin_tab:`mxnet`
[Discussions](https://discuss.d2l.ai/t/23)
:end_tab:

:begin_tab:`pytorch`
[Discussions](https://discuss.d2l.ai/t/24)
:end_tab:

:begin_tab:`tensorflow`
[Discussions](https://discuss.d2l.ai/t/436)
:end_tab:
