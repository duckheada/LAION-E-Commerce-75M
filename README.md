# LAION-E-Commerce-75M

LAION-E-Commerce is a set of 75M E-commerce images mined from LAION-2B-en, using a [SNIP](https://github.com/ryanwebster90/snip-dedup) index, and using 300k samples from [XMRec](https://xmrec.github.io/) as a "seed" dataset. Generic product information has been transfered as a new column in the parquet. 

Here is the [LAION-E-Commerce-75M](https://huggingface.co/datasets/fraisdufour/LAION_ecommerce) dataset on huggingface, you may download with

You may download the parquet files with
```python
from huggingface_hub import snapshot_download
snapshot_download(repo_id="fraisdufour/LAION_ecommerce")
```

## Roadmap

Stay tuned for new versions!
- [x] V1: expand the "seed" dataset of XMRec to L2B
- [ ] SNIP indices for dataset exploration
- [ ] Google colab for dataset exploration
- [ ] More "generic" meta data transfered, e.g. product specifications
- [ ] Releasing a larger set, and evaluating the quality (e.g. w.r.t. downstream tasks)
