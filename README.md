# Computer Vision

Kompyuter ko'rish bo'yicha Colab notebooklarim.

## Vegetable Image Dataset

[vegetable_dataset.ipynb](vegetable_dataset.ipynb) notebookini [Colab'da oching](https://colab.research.google.com/github/Sanjarbek9706/computer_vision/blob/main/vegetable_dataset.ipynb) va kataklarni yuqoridan pastga ishga tushiring.

Notebook quyidagilarni bajaradi:

1. Kaggle'dagi [Vegetable Image Dataset](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset) 1-versiyasini `kagglehub` orqali Colab'ga yuklaydi.
2. `train`, `validation`, `test` bo'limlari va 15 ta sinf bir xil ekanini tekshiradi.
3. Har bir rasmning bo'limi, sinfi va nisbiy yo'lini `/content/vegetable_manifest.csv` fayliga yozadi.
4. Har bir bo'lim va sinfdan namunaviy rasmlarni ochib tekshiradi hamda PyTorch `ImageFolder` / `DataLoader` obyektlarini yaratadi.

Kaggle sahifasiga ko'ra, datasetda 21 000 ta JPG rasm bor: 15 000 ta train, 3 000 ta validation va 3 000 ta test. Rasmlar GitHub reposiga ko'chirilmagan; notebook ularni ishga tushirilganda oladi. `vegetable_manifest.csv` Colab sessiyasida yaratiladi.

Bu datasetda piyoz, sarimsoq, guruch va go'sht sinflari yo'q. Uydagi mahsulotlardan retsept tavsiya qilish loyihasida bu mahsulotlarni qo'lda kiritish yoki qo'shimcha dataset bilan kengaytirish kerak. Bitta suratdagi bir nechta mahsulotni aniqlash uchun keyinroq object detection modeli kerak bo'ladi.

**Manba va litsenziya:** M Israk Ahmed, Shahriyar Mahmud Mamun va Asif Uz Zaman Asif, “DCNN-Based Vegetable Image Classification Using Transfer Learning: A Comparative Study” (ICCCSP, 2021); dataset [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
