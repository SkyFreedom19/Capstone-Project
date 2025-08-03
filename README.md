# Capstone-Project
Analysis Laptop Price using LLM ibm granite

# Title Project
Analysis Laptop Price Using LLM IBM Granite

# Raw Dataset Link
https://www.kaggle.com/datasets/owm4096/laptop-prices/data

# Project Overview
Tujuan: Pengumpulan spesifikasi laptop untuk inventarisasi, perbandingan, atau tinjauan teknis/analisis pasar.
Latar Belakang: Bagian dari dataset atau proyek yang berfokus pada spesifikasi laptop, mungkin untuk dokumentasi, penelitian, atau tujuan pendidikan.
Masalah Khusus: Diperkirakan sebagai masalah umum yang diatasi oleh spesifikasi detail (misalnya, optimasi kinerja, pemeriksaan kompatibilitas, mengidentifikasi laptop untuk kebutuhan pengguna tertentu).
Pendekatan: Pengumpulan dan pengorganisasian sistematis spesifikasi detail dalam format terstruktur (pandas DataFrame) untuk akses dan perbandingan yang mudah.

# Insight & Findings
Perusahaan Unik: Apple, HP 
Jenis Unik: Ultrabook, Notebook 
Perusahaan CPU Unik: Intel, AMD (Intel lebih umum) 
Perusahaan GPU Unik: Intel, AMD (Intel lebih umum) 
Penyimpanan Utama: 3 SSD, 1 Penyimpanan Flash 
Penyimpanan Sekunder: 4 tanpa penyimpanan sekunder, 1 dengan ‘Tidak’ penyimpanan sekunder 

Temuan ini memberikan gambaran yang jelas tentang model laptop yang termasuk dalam dataframe, produsennya, dan konfigurasi penyimpanannya.

# AI Support Explanation
Untuk menjelaskan bagaimana model bahasa seperti saya dapat digunakan untuk menganalisis data teks yang berkaitan dengan laptop, seperti ulasan atau deskripsi, ikuti langkah-langkah berikut:: 
Install TextBlob (run this in a separate code cell): ```bash !pip install textblob ``` 
Import TextBlob and perform sentiment analysis: ```python 
from textblob import TextBlob 
# Hypothetical textual data for demonstration 
df_text = pd.DataFrame({ 
'description': [ 
'The Apple MacBook Pro is an excellent machine with a stunning Retina display.’, 
'HP 250 G6 is a solid budget laptop with decent performance.’, 
'The MacBook Air is lightweight and portable but lacks power.’, 
'Apple MacBook Pro with AMD Radeon Pro offers impressive graphics for professionals.’, 
'MacBook Pro delivers good performance with its Intel Core processors.’ 
] 
}) 
# Perform sentiment analysis 
df_text['sentiment'] = df_text['description'].apply(lambda x: TextBlob(x).sentiment.polarity) 

# Display the dataframe with sentiment scores 
print(df_text[['description', 'sentiment']]) 
``` 
Kode ini akan menambahkan kolom ‘sentimen’ ke dataframe, menghitung polaritas sentimen untuk setiap deskripsi laptop menggunakan TextBlob. Skor polaritas berkisar dari -1 (paling negatif) hingga 1 (paling positif).
Perlu diingat, contoh ini menggunakan deskripsi hipotetis karena dataframe asli `df` hanya berisi data numerik dan kategorikal, bukan teks yang cocok untuk analisis sentimen. Dalam skenario dunia nyata, Anda akan mengganti deskripsi hipotetis dengan data teks aktual dari ulasan atau deskripsi produk.
Untuk dataframe asli Anda, karena tidak mengandung data teks, model bahasa seperti saya tidak dapat diterapkan langsung untuk tugas-tugas seperti klasifikasi, ringkasan, atau analisis sentimen. Model bahasa memerlukan masukan teks untuk melakukan tugas-tugas semacam ini.
```

# Visualization 
<img width="561" height="412" alt="image" src="https://github.com/user-attachments/assets/a73c0dbc-7566-4bda-bd67-7054187ab065" />

<img width="1023" height="564" alt="Screenshot 2025-08-03 194211" src="https://github.com/user-attachments/assets/1697d4e8-0ba3-4b82-a2e5-d66ad72c0677" />



