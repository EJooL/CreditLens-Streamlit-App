# 🔍 CreditLens — Credit Risk Analytics

Aplikasi web analisis risiko kredit berbasis machine learning.  
UAS Data Mining · Sistem Informasi UNESA · 2024/2025

## Struktur Folder

```
UAS_DataMining_NamaKelompok/
├── dataset/
│   └── cs-training.csv          ← letakkan di sini
├── model/
│   ├── kmeans_final.pkl          ← export dari notebook
│   ├── scaler_cluster.pkl
│   └── cluster_metadata.json
├── app/
│   ├── app.py                    ← entry point
│   └── pages/
│       ├── 1_home.py
│       ├── 2_dataset.py
│       ├── 3_prediction.py
│       ├── 4_visualization.py
│       └── 5_about.py
├── notebook/
│   └── UASMINING_clustering.ipynb
├── requirements.txt
└── README.md
```

## Cara Menjalankan

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Letakkan model hasil notebook ke folder model/
#    (kmeans_final.pkl, scaler_cluster.pkl, cluster_metadata.json)

# 3. Letakkan cs-training.csv ke folder dataset/

# 4. Jalankan aplikasi
cd app
streamlit run app.py
```

## Deployment Online (Streamlit Cloud)

1. Push repo ke GitHub
2. Buka https://share.streamlit.io
3. Connect repo, set `app/app.py` sebagai entry point
4. Deploy

## Fitur Aplikasi

| Halaman | Isi |
|---------|-----|
| 🏠 Home | Deskripsi proyek, statistik kunci, tim |
| 📊 Dataset Overview | EDA, distribusi, heatmap korelasi |
| 🔮 Prediction & Analysis | Form input nasabah, prediksi segmen, rekomendasi |
| 📈 Visualization | Cluster analysis, radar chart, evaluasi model |
| ℹ️ About | Metodologi, tech stack, dokumentasi |
