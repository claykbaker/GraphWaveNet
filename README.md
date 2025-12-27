## GraphWaveNet (GWNet) Baseline Model Results

This folder contains results for a trained GWNet model and its incremental improvement. 

The implementation for the former is based on the IJCAI 2019 paper “Graph WaveNet for Deep Spatial-Temporal Graph Modeling” (https://arxiv.org/abs/1906.00121), with the following citation:

```bibtex
@article{wu2019graph,
  title={Graph wavenet for deep spatial-temporal graph modeling},
  author={Wu, Zonghan and Pan, Shirui and Long, Guodong and Jiang, Jing and Zhang, Chengqi},
  journal={arXiv preprint arXiv:1906.00121},
  year={2019}
}
```

The implementation for the latter is based on the arXiv 2019 paper “Incrementally Improving Graph WaveNet Performance on Traffic Prediction” (https://arxiv.org/abs/1912.07390), with the following citation:

```bibtex
"@article{shleifer2019incrementally,
  title={Incrementally improving graph wavenet performance on traffic prediction},
  author={Shleifer, Sam and McCreery, Clara and Chitters, Vamsi},
  journal={arXiv preprint arXiv:1912.07390},
  year={2019}
}"
```

### Files
- `best_model.pth`: PyTorch checkpoint of the trained model
- `test.csv`: Test set predictions and ground truth
- `metrics.csv`: Evaluation metrics on the test set
- `args.pkl`: Pickled Python object storing the full set of training arguments
  (model architecture, optimisation hyperparameters, data settings, random seed)
  used to produce `best_model.pth`

### Environment
- Python:  3.9
- PyTorch: 1.10.2
- Device: MPS (Apple Silicon)
- Conda environment exported in `environment.yml`
