# Pre-entrega 1: Pipeline de entrenamiento, validación y clasificador base

## 🛠️ Configuración del Experimento
- **Versión de PyTorch:** `2.11.0+cpu`
- **Dispositivo utilizado:** `cpu`
- **Optimizador:** Adam
- **Learning Rate elegido:** `0.01`
- **Arquitectura:** MLP (`4 -> 16 -> 16 -> 3`) con activaciones `ReLU`.

## 📈 Resultados y Lectura de la Curva de Pérdida
- **Pérdida inicial (Época 1):** Train `1.0109` | Validación `0.8613`
- **Pérdida final (Época 50):** Train `0.0242` | Validación `0.0946`
- **Accuracy final en Validación:** `96.67%`

### Interpretación del experimento:
La pérdida (*loss*) descendió de manera consistente a lo largo de las 50 épocas tanto en el conjunto de entrenamiento como en el de validación. Ambas curvas convergen de forma pareja sin que la pérdida de validación se dispare hacia arriba, lo que demuestra que el clasificador base aprende patrones generalizables y no presenta *overfitting* severo.