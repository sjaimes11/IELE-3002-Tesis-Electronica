# Rutinas de entrenamiento y evaluación (ViT, Swin, MobileNetV3 y ResNet18) — Tesis IELE-3002

Este repositorio contiene las rutinas de preprocesamiento, entrenamiento y evaluación usadas en mi tesis para analizar micrografías **EFM-2ωe** y entrenar modelos de visión por computador con el fin de predecir parámetros de fabricación (p. ej., **voltaje** y **frecuencia**).

> Nota: El archivo principal de trabajo es el notebook:
> **`Rutina_para_ViT_Swin_y_MobileNet.ipynb`**
> (en este notebook están organizadas las secciones por tarea y por arquitectura).

---

## ¿Qué hay en este repositorio?

### 1) Notebook principal (rutinas de modelos)
En `Rutina_para_ViT_Swin_y_MobileNet.ipynb` encontrarás secciones como:

- **Reescalado de imágenes** (ej. de 1024×1024 a 224×224 para modelos tipo ViT/Swin).
- **Predicción por Voltaje** (clasificación) con:
  - ViT (incluye variante “aumentada”)
  - Swin Transformer (incluye variante “aumentada”)
  - MobileNetV3
  - ResNet18 (incluye variante “aumentada”)
- **Predicción por Frecuencia** (clasificación) con:
  - ViT (normal y “aumentado”)
  - Swin (normal y “aumentado”)
  - MobileNetV3
  - ResNet18 (normal y “aumentado”)


---

## Requisitos

Este proyecto fue ejecutado principalmente en **Google Colab**.

### Librerías típicas usadas
- `torch`, `torchvision`
- `timm`
- `pandas`, `numpy`
- `scikit-learn`
- `torchmetrics`
- `opencv-python`
- `matplotlib`, `seaborn`
- `tqdm`

En Colab, normalmente basta con instalar (si no vienen preinstaladas):
```bash
pip install timm pandas scikit-learn pillow tqdm torchmetrics opencv-python
