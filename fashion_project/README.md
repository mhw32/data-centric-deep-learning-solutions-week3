# Week 3 Project: Active learning on fashion classifier

```
pip install -e .
```

This project will investigate various strategies to identify elements for relabeling.

### Instructor notes

- The repo comes with a `data/production/dataset.pt` file. To generate this, run `create_prod_data.py`. Using the `checkpoints/model.ckpt`, you get 30.2%.
- The repo comes with a `checkpoints/model.ckpt` file. To generate this, run `python scripts/train.py run` and move the best checkpoint to the `checkpoints` folder. This checkpoint should get 85.2% on the FashionMNIST test set.

### Finetuning results

| model | prod acc |
| --- | --- |
| none | 30.2% |
| random | 38.9% |
| uncertainty | 34.0% | 
| margin | 37.5% | 
| entropy | 42.4% |
| augment | |