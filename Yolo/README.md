# Обучение YOLO

- [`YOLO_MOD.ipynb`](YOLO_MOD.ipynb) — код подготовки датасета и обучения YOLOv8n на размеченных данных из [`../Razmetka_manual`](../Razmetka_manual).
- [`best_yolo_model.pt`](best_yolo_model.pt) — лучшие веса обученной модели (сохраняются кодом в `/content/drive/MyDrive/best_yolo_model.pt`).
- [`metrics/`](metrics/) — графики и логи обучения (results.csv, results.png, confusion matrix, PR/P/R-кривые, val_batch2_labels.jpg, val_batch2_pred.jpg).

## Параметры обучения

- Эпохи: 80
- Batch: 32
- Платформа: GPU
- Выходные данные: `/content/runs/detect/yolo/bubbles_text/weights/`

## Как воспроизвести обучение

1. Скачать датасет по ссылке из [`../Razmetka_manual/README.md`](../Razmetka_manual/README.md), положить в `/content/drive/MyDrive/Base.zip` (Google Colab).
2. Запустить `YOLO_MOD.ipynb` — обучится модель, веса появятся в `/content/runs/detect/yolo/bubbles_text/weights/best.pt` и будут скопированы в `/content/drive/MyDrive/best_yolo_model.pt`.

> Повторное обучение не обязательно — в репозитории уже лежат готовые веса (`best_yolo_model.pt`) и все метрики/графики обучения для ознакомления (папка `metrics/`).
