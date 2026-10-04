# datasets

This repo holds the image data for
[Chicken-disease-classification-project](https://github.com/mhussainahmad/Chicken-disease-classification-project),
an image classifier that labels chicken fecal images as healthy or coccidiosis.

## Contents

`Chicken-fecal-images.zip` (about 11 MB compressed) contains 390 RGB JPEG images, all 224x224 pixels, in two class folders:

```
Chicken-fecal-images/
  Coccidiosis/   195 images (cocci.<n>.jpg)
  Healthy/       195 images (healthy.<n>.jpg)
```

The two classes are the same size. The archive has no predefined train/validation/test split.

## Usage

The project's data ingestion stage downloads the archive from this URL (set in its `config/config.yaml`):

```
https://github.com/mhussainahmad/datasets/raw/main/Chicken-fecal-images.zip
```

To get it manually:

```bash
curl -L -o Chicken-fecal-images.zip https://github.com/mhussainahmad/datasets/raw/main/Chicken-fecal-images.zip
unzip Chicken-fecal-images.zip
```

The original source and licence of the images are not recorded in this repository.
