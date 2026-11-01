# PhyVLM-CR

Code and project page for **Physics-Guided VLM Priors for All-Cloud Removal** by Liying Xu, Huifang Li, and Huanfeng Shen, published in *IEEE Geoscience and Remote Sensing Letters* (2026). [Paper](https://ieeexplore.ieee.org/abstract/document/11641653).

## Colab notebook

Open [`PhyVLM_CR6_Colab.ipynb`](PhyVLM_CR6_Colab.ipynb) in Google Colab and run cells in order. Before running, add these two entries in **Colab → Secrets** and grant the notebook access:

- `EE_PROJECT_ID`: your Google Earth Engine Cloud project ID.
- `DASHSCOPE_API_KEY`: your DashScope API key for Qwen-Image-Edit-Plus.

The notebook downloads Sentinel-2 observations through Earth Engine, obtains the VLM cognitive prior from DashScope, estimates atmospheric light and transmission, performs transmission-guided restoration and temporal fusion, evaluates the output, and exports figures/data. You need access to both external services. Results can vary with available scenes and the external VLM service. The included images and metrics are reproduced from the supplied manuscript; they are not a fresh run of the public notebook.

**Do not commit credentials, saved notebook outputs, account files, or downloaded scene data.** The released notebook contains no execution outputs or embedded credentials.

## Project page

The static page is in [`docs/`](docs/index.html). For GitHub Pages, publish the `docs/` folder on the default branch.

## Scope

This public package contains the Colab CR6 workflow and the paper figures used on the project page. The legacy local scripts and previous exploratory notebooks are not part of the release.

## License

The code is available under the [Apache License 2.0](LICENSE). Figures reproduced from the manuscript remain credited to the paper authors.

## Citation

```bibtex
@article{Xu_2026,
  title={Physics-Guided VLM Priors for All-Cloud Removal},
  author={Xu, Liying and Li, Huifang and Shen, Huanfeng},
  journal={IEEE Geoscience and Remote Sensing Letters},
  volume={23},
  pages={6017305--6017305},
  year={2026},
  doi={10.1109/LGRS.2026.3720251}
}
```
