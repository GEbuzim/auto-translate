# Датасет (Labeling.zip)

Размеченный датасет для обучения YOLO (765 изображений манги в `jpeg` + YOLO-разметка на 2 класса: `bubbles`, `text`) слишком большой (~126 МБ), чтобы хранить его в git-репозитории напрямую.

**Ссылка на скачивание (Google Drive):** https://drive.google.com/file/d/1a7WXl_SshpG62kNVQB_fQ_SN-hfJ64pe/view?usp=sharing

## Структура архива

```
Labeling.zip
├── converted_images/   # 765 изображений jpeg
└── labels/              # YOLO-разметка (.txt), классы: 0 - bubbles, 1 - text
```

Чтобы использовать датасет для обучения (см. `training/Yolo_V.ipynb`):
1. Скачайте `Labeling.zip` по ссылке выше.
2. В Google Colab положите файл в `/content/drive/MyDrive/Labeling.zip`.
3. Запустите `training/Yolo_V.ipynb` — он сам подмонтирует Google Drive и распакует архив.
