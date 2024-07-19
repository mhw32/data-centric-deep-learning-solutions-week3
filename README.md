# DCDL Solutions Week 3
Solutions for DCDL uplimit course (Week 3)

### Setup

- For each project repository, install it by running `pip install -e .` from within the folder.
- For the confidence learning project, please download a dataset of recomputed embeddings [here](https://drive.google.com/file/d/12UtQMwfSgm4FpXSFZvLDNLO8VGxzCPYq/view?usp=sharing). Please `conflearn_project/data` with the unzipped file.
- The repo comes with a `data/production/dataset.pt` file. To generate this, run `create_prod_data.py`. Using the `checkpoints/model.ckpt`, you get 30.2%.
- The repo comes with a `checkpoints/model.ckpt` file. To generate this, run `python scripts/train.py run` and move the best checkpoint to the `checkpoints` folder. This checkpoint should get 85.2% on the FashionMNIST test set.
