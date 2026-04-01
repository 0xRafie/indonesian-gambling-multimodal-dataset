# Indonesian Online Gambling Promotion Multimodal Dataset

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

Posts were collected from Facebook, TikTok, and X using various gambling-related keywords, including but not limited to "Judi Online," "Judol," and "Slot Gacor." After deduplication and filtering, the authors manually annotated each sample as gambling promotion (1) or non-gambling (0).

## License

This dataset is released under the [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.
