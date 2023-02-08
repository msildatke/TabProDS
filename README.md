# TabProDS

TabProDS is the accompanying dataset for the paper on "TabProIS: A Transfer Learning-Based Model for Detecting Tables in Product Information Sheets". It consists of 5,600 document images which were converted from Product Information Sheets. Out of these, 4,489 images contain at least one table. A table can have a wide variety of layouts, ranging from full grid-style borders to no borders at all. The layout of the document pages also varies. We tried to ensure that not too many document images with a similar layout bias the dataset.

![Example documents](/resources/example.png?raw=true "Examples documents")

If you want to reuse our work, please cite it. An exemplary BibTex entry is listed at the bottom of this page.

## Annotation Format

The images are annotated in the standard COCO format.

## Splits

The dataset is split into three parts:

- 3920 (70%) images for training
- 840 (15%) images for development
- 840 (15%) images for validation

## Resolution

The individual images were converted from PDF files in two different resolutions.

### Full Resolution (300 dpi)

The full resolution images typically have the dimensions 2480x2509 pixels (portrait). Some might have a landscape orientation or different dimensions as well as different aspect ratios altogether.

In total, the full resolution dataset is 3.9 GB in size with an average of 670 kB per image.

### Reduced Resolution (75 dpi)

The reduced resolution images are a sixteenth the size of their full resolution counterparts. This results in the typical dimensions of 620x877 pixels. Again, these dimensions are not guaranteed as some images might be in landscape orientation or a different size and aspect ratio.

The reduced resolution dataset weighs in at 344 MB with an average of 62 kB per image.

## File Structure

```
.
├── img                          # all images
│   ├── full                     # full resolution (300 dpi) images  (coming soon)
│   │   ├── P000053802-1.jpg
│   │   ├── ... (5598 more)
│   │   └── P000237430-2.jpg
│   └── reduced                  # reduced resolution (150 dpi) images
│       ├── P000053802-1.jpg
│       ├── ... (5598 more)
│       └── P000237430-2.jpg
├── dev.full.json                # full resolution development set annotations
├── dev.reduced.json             # reduced resolution development set annotations
├── README.md                    # this README file
├── train.full.json              # full resolution training set annotations
├── train.reduced.json           # reduced resolution training set annotations
├── val.full.json                # full resolution validation set annotations
└── val.reduced.json             # reduced resolution validation set annotations
```

## Cite This

```tex
@article {
    # ... coming soon
}
```