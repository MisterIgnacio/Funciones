Este proyecto es una aplicación de consola interactiva escrita en Python que permite a los surfistas evaluar las condiciones del mar y del viento antes de entrar al agua. El programa calcula la viabilidad del surf, alerta sobre condiciones meteorológicas peligrosas y ofrece recomendaciones sobre el equipo adecuado según la temperatura.

## 🌟 Características

El script principal ofrece un menú interactivo con las siguientes funcionalidades:
1. **Evaluar si el mar es surfeable:** Determina si la altura de la ola es adecuada.
2. **Evaluar peligro de viento:** Alerta sobre ráfagas de viento que puedan comprometer la seguridad.
3. **Consultar límite de temperatura:** Informa sobre la temperatura crítica del agua y la necesidad de usar trajes de neopreno gruesos (ej. 4/3mm).
4. **Ver aviso de la Armada:** Muestra alertas oficiales respecto a marejadas u otras contingencias.
5. **Actualizar datos:** Permite modificar las condiciones de la ola y el viento sin reiniciar el programa.
6. **Salir:** Finaliza la ejecución de la aplicación.

## 📁 Estructura del Proyecto

Para que este script funcione correctamente, se asume que el proyecto cuenta con la siguiente estructura de módulos:

* `main.py`: Archivo principal que contiene el flujo de ejecución y el menú interactivo (código proporcionado).
* `calculos.py`: Módulo encargado de la lógica de negocio y validaciones. Debe exportar:
    * `es_surfeable(altura_ola)`
    * `alertar_viento_peligroso(viento)`
    * `obtener_temperatura_limite_traje()`
    * `mostrar_advertencia_marejada()`
* `pantalla.py`: Módulo encargado de la interfaz visual en consola. Debe exportar:
    * `mostrar_titulo()`
    * `titulo_menu()`

## 🚀 Requisitos e Instalación

1. Asegúrate de tener instalado **Python 3.x** en tu sistema.
2. Clona o descarga los archivos del proyecto en un mismo directorio.

```bash
git clone [https://github.com/tu-usuario/asistente-surf.git](https://github.com/tu-usuario/asistente-surf.git)
cd asistente-surf
