# ACADEMIC RESEARCH DATASET - FOR DETECTING GAMBLING SPAM

**This repository contains a machine learning research dataset for DETECTING and FILTERING online gambling promotions on Indonesian social media. This is NOT a gambling website or promotional content.**

---

## Research Context

This dataset is created for **academic research** in harmful content detection and multimodal machine learning. It is intended to help platforms and researchers develop AI systems to identify and remove gambling spam - not to promote gambling.

- **Research Paper:** Unpublished research project
- **License:** CC BY-NC 4.0 (annotations and metadata)
- **Institution:** Institut Teknologi Sepuluh Nopember

## What This Dataset Is

- **Purpose:** Train ML models to identify gambling promotions vs. legitimate content
- **Content:** 5,028 annotated social media posts (gambling spam samples + non-gambling samples)
- **Use Case:** Binary classification for content moderation systems
- **Precedent:** Similar to spam detection datasets, phishing email datasets, malware analysis datasets - standard in cybersecurity and NLP research

## What This Dataset Is NOT

- This is NOT a gambling website
- This is NOT promotional content for gambling
- This is NOT intended for commercial gambling operations
- This does NOT encourage or facilitate gambling

---

## Indonesian Online Gambling Promotion Multimodal Dataset

A multimodal dataset of 5,028 annotated social media posts for detecting online gambling promotions in Indonesia, containing paired images and Indonesian text captions collected from Facebook, TikTok, and X.

## Dataset Statistics

| Platform | Gambling | Non-Gambling | Total |
|----------|----------|--------------|-------|
| Facebook | 927 | 492 | 1,419 |
| TikTok | 199 | 1,243 | 1,442 |
| X | 1,069 | 1,098 | 2,167 |
| **Total** | **2,195 (43.7%)** | **2,833 (56.3%)** | **5,028** |

## Data Format

```
data/
├── dataset.csv      # Annotations and metadata
└── image/           # 5,028 images
    ├── image_1.jpg
    ├── image_2.jpg
    └── ...
```

**Columns in `dataset.csv`:**

| Column | Type | Description |
|--------|------|-------------|
| `id` | int | Unique sample ID |
| `text_caption` | str | Indonesian text caption from the post |
| `image_path` | str | Relative path to the image file (e.g., `image/image_1.jpg`) |
| `platform` | str | Source platform: `Facebook`, `TikTok`, or `X` |
| `url` | str | Original post URL |
| `label` | float | `1.0` = gambling promotion, `0.0` = non-gambling |

## Collection Method

Posts were collected from Facebook, TikTok, and X using various gambling-related keywords for research purposes only. After deduplication and filtering, the authors manually annotated each sample as gambling promotion (1) or non-gambling (0).

## Ethics Statement

- All data was collected from publicly available sources
- No private or personal data was intentionally collected  
- The dataset is intended solely for academic and research purposes in content moderation
- This dataset follows standard practices for research datasets in machine learning and cybersecurity

## Intended Use

**This dataset is intended for:**
- Machine learning research
- Content moderation system development
- Harmful content detection research

**This dataset is NOT intended for:**
- Promoting or facilitating gambling
- Commercial gambling operations
- Redistributing gambling content for promotional purposes

## Citation

If you use this dataset in your research, please cite:

> Ekaputra, D. R. (2026). *Indonesian Online Gambling Promotion Multimodal Dataset* [Data set]. GitHub. https://github.com/0xRafie/indonesian-gambling-multimodal-dataset
> 
> **Note:** This dataset is part of an unpublished research project at Institut Teknologi Sepuluh Nopember.

## License

The annotations and metadata (`dataset.csv`) are released under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): you may share and adapt them for non-commercial purposes, with attribution.

The images and captions come from public posts on Facebook, TikTok, and X. They remain the property of their original owners and are included only for non-commercial research. If you own a post in this dataset and want it removed, open an issue and it will be taken down.

**Note:** This license does not grant permission to use the dataset for illegal activities or gambling promotion.

---

## For GitHub Support

This repository contains a research artifact for machine learning classification of harmful content. It is analogous to phishing detection datasets, spam classification datasets, and malware analysis datasets commonly hosted on GitHub for academic research. The dataset is not intended to promote gambling but to help detect and filter gambling spam on social media platforms.