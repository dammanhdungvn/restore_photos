.
├── README.md
├── code: Nơi chứa file code
│   ├── main.ipynb
│   └── split_images.ipynb
├── images: Nơi chứa file ảnh
│   ├── origin: Ảnh gốc download trên mạng, có thể không đúng kích thước 600*360 cũng được
│   │   ├── origin1.png
│   │   ├── origin2.png
│   │   ├── origin3.png
│   │   ├── origin4.png
│   │   ├── origin5.png
│   │   └── origin6.png
│   ├── problem: Những bức ảnh sẽ được xáo cho các task, nơi mô hình sẽ xử lý bức ảnh này để khôi phục
│   │   ├── task1
│   │   │   ├── origin1.png
│   │   │   ├── origin2.png
│   │   │   ├── origin3.png
│   │   │   ├── origin4.png
│   │   │   ├── origin5.png
│   │   │   └── origin6.png
│   │   └── task2
│   │       ├── origin1.png
│   │       ├── origin2.png
│   │       ├── origin3.png
│   │       ├── origin4.png
│   │       ├── origin5.png
│   │       └── origin6.png
│   ├── resize: Đọc ảnh gốc sau đó resize lại nếu bức ảnh có kích thước vượt quá 600*360
│   │   ├── origin1.png
│   │   ├── origin1_600x360.png
│   │   ├── origin2.png
│   │   ├── origin2_600x360.png
│   │   ├── origin3.png
│   │   ├── origin3_600x360.png
│   │   ├── origin4.png
│   │   ├── origin4_600x360.png
│   │   ├── origin5.png
│   │   ├── origin5_600x360.png
│   │   ├── origin6.png
│   │   └── origin6_600x360.png
│   └── sloved: Mô hình khôi phục lại ảnh problem
│       ├── task1
│       │   ├── origin1.png
│       │   ├── origin2.png
│       │   ├── origin3.png
│       │   ├── origin4.png
│       │   ├── origin5.png
│       │   └── origin6.png
│       └── task2
│           ├── origin1.png
│           ├── origin2.png
│           ├── origin3.png
│           ├── origin4.png
│           ├── origin5.png
│           └── origin6.png
├── output: Chứa các file cần phải submit cho ban tổ chức
│   ├── output.csv
│   ├── permutations
│   │   ├── origin1.json
│   │   ├── origin2.json
│   │   ├── origin3.json
│   │   ├── origin4.json
│   │   ├── origin5.json
│   │   └── origin6.json
│   ├── run.log
│   └── submission.zip
└── requirements.txt

13 directories, 55 files