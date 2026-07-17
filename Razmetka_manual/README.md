# Разметка датасета (Base.zip)

Размеченный датасет для обучения YOLO: 670 изображений манги в `JPEG` + YOLO-разметка на 2 класса (`0 — speech bubble`, `1 — text`).

**Ссылка на скачивание (Google Drive):** https://drive.google.com/file/d/1y8EVeMEQaMLT3bqHKzt3uZZMMUas1EbO/view?usp=sharing

## Структура архива

```
Base.zip
├── images/   # 670 изображений JPEG
└── labels/    # YOLO-разметка (.txt), классы: 0 - speech bubble, 1 - text
```

Чтобы использовать датасет для обучения (см. [`../Yolo/YOLO_MOD.ipynb`](../Yolo/YOLO_MOD.ipynb)):
1. Скачайте `Base.zip` по ссылке выше.
2. В Google Colab положите файл в `/content/drive/MyDrive/Base.zip`.
3. Запустите `Yolo/YOLO_MOD.ipynb` — он сам подмонтирует Google Drive и распакует архив.
