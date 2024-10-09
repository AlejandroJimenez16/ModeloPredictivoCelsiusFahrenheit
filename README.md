# Prediccion de grados Celsius a Fahrenheit

Este programa utiliza TensorFlow y Keras para predecir los grados fahrenheit, basándose en grados celsius. El modelo se entrena con un conjunto de datos simple y realiza predicciones al final del entrenamiento.

## Descripción

El modelo se basa en una red neuronal que toma como entrada:

- **Grados Celsius**: Grados Celsius.

A partir de estas entradas, el modelo predice:

- **Grados fahrenheit**: Grados Fahrenheit.

## Tecnologías utilizadas

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib

## Instalación

Para ejecutar este programa, asegúrate de tener instalado Python 3.x. Luego, puedes instalar las dependencias necesarias utilizando `pip`:

```bash
  pip install tensorflow numpy matplotlib
```

## Uso

1. **Ejecuta el código:** Simplemente ejecuta el archivo Python que contiene el código.
2. **Entrenamiento:** El modelo se entrenará durante 1000 épocas. Durante este proceso, podrás ver cómo se reduce la magnitud de pérdida.
3. **Predicción:** Una vez que el modelo ha sido entrenado, puedes hacer una predicción ingresando un numero de grados celius. En el código proporcionado, se realiza una predicción para 31 grados:
   
   ```python
   resultado = modelo.predict(np.array([31.0]))
   print("El resultado es " + str(resultado) + " fahrenheit!")
   ```

## Resultados

El programa generará una gráfica que muestra la magnitud de pérdida a lo largo de las épocas. También imprimirá lod grados fahrenheit correspondientes.

![image](https://github.com/user-attachments/assets/29d195eb-01ba-46d1-a562-683df7d1f333)

## Ejemplo de salida

```plainText
===========================
Comenzando entrenamiento...
===========================
=================
Modelo entrenado!
=================
Hagamos una predicción!
==================================================
El resultado es [[87.6889]] fahrenheit!
==================================================
```

## Guardar el modelo

Esta linea es la que se encarga de guardar el modelo, si deseea otra ruta puede cambiarla:

```python
modelo.save("modeloPrediccionSuenio.keras")
```

