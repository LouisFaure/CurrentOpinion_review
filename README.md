# Current Opinion review code

## Obtaining data

```bash
git clone https://github.com/LouisFaure/CurrentOpinion_review/
cd CurrentOpinion_review/
wget https://figshare.com/ndownloader/files/36201420 -O Hippocampus/DentateGyrus.loom
wget https://figshare.com/ndownloader/files/37334341 -O ENS/morarach20.h5ad
```

## Creating environment

```bash
mamba create -n scFates -c conda-forge -c r -c bioconda \
    python=3.8 r-mgcv rpy2=3.4.3 jupyter ipykernel anndata2ri -y

pip install scFates scvelo
```