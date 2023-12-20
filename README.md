## PTF Classification

---
### This project detects whether the images have a hamlet or not
```
dls = ImageDataLoaders.from_folder(
    path=DATASET_PATH,
    item_tfms=Resize(224),
    bs=16,
    batch_tfms=[Normalize.from_stats(*imagenet_stats), RandTransform()],
    valid_pct=0.2
)
dls.show_batch()
```

![image](https://github.com/DataAzat/PTF-Classification/assets/147945113/dfed8566-c181-4a17-9bfb-3468a1f285cd)
