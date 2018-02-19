<h1>DiversityNet</h1>

DiversityNet is a benchmarking platform to support research on open-domain molecule generation models. DiversityNet is not only implementing a majority of molecule generation models, but also covered a set of metrics that evaluate the diversity, the quality and the consistency of the generated molecules. The DiversityNet platform could help standardize the research on molecule generation and facilitate the sharing of fine-tuned open-source implementations among researchers and practitioners for their work.  As a consequence, this would help in improving the reproductivity and reliability of future research work in molecule generation.

For more details, please refer to our Authorea paper: [Texygen: A Benchmarking Platform for Text Generation Models](https://arxiv.org/abs/1802.01886) by Yaoming Zhu et al. 2018.

Should you have any questions and enquiries, please feel free to contact on Telegram Yaoming Zhu (ym-zhu [AT] outlook.com) and [Weinan Zhang](http://wnzhang.net) (wnzhang [AT] sjtu.edu.cn).

## Requirement
We suggest you run the platform under Python 3.6+ with following libs:
* **TensorFlow 1.3.0**
* Numpy 1.12.1
* Scipy 0.19.0
* NLTK 3.2.3
* CUDA 7.5+ (Suggested for GPU speed up, not compulsory)    

Or just type `pip install -r requirements.txt` in your terminal.

## Implemented Models and Original Papers

* **SeqGAN** -  [SeqGAN: Sequence Generative Adversarial Nets with Policy Gradient](https://arxiv.org/abs/1609.05473)

* **MaliGAN** - [Maximum-Likelihood Augmented Discrete Generative Adversarial Networks](https://arxiv.org/abs/1702.07983)

* **RankGAN** - [Adversarial ranking for language generation](http://papers.nips.cc/paper/6908-adversarial-ranking-for-language-generation)

* **LeakGAN** - [Long Text Generation via Adversarial Training with Leaked Information](https://arxiv.org/abs/1709.08624)

* **TextGAN** - [Adversarial Feature Matching for Text Generation](https://arxiv.org/abs/1706.03850)
 
* **GSGAN** - [GANS for Sequences of Discrete Elements with the Gumbel-softmax Distribution](https://arxiv.org/abs/1611.04051)


## Get Started

```bash
git clone https://github.com/geek-ai/Texygen.git
cd Texygen
# run SeqGAN with default setting
python3 main.py
```
More detailed documentation for the platform and code setup is provided [here](docs/doc.md).


## Evaluation Results

BLEU on image COCO caption test dataset:

|       | SeqGAN | MaliGAN | RankGAN | LeakGAN | TextGAN      | MLE |
|-------|--------|---------|---------|---------|--------------|--------------|
| BLEU2 | 0.745  | 0.673   | 0.743   | 0.746   | 0.593        | 0.731        |
| BLEU3 | 0.498  | 0.432   | 0.467   | 0.528   | 0.463        | 0.497        |
| BLEU4 | 0.294  | 0.257   | 0.264   | 0.355   | 0.277        | 0.305        |
| BLEU5 | 0.180  | 0.159   | 0.156   | 0.230   | 0.207        | 0.189        |

Mode Collapse (Self-BLEU):

|            | SeqGAN | MaliGAN | RankGAN | LeakGAN | TextGAN       | MLE  |
|------------|--------|---------|---------|---------|---------------|--------------|
| BLEU2      | 0.950  | 0.918   | 0.959   | 0.966   | 0.942         |0.916         |
| BLEU3      | 0.840  | 0.781   | 0.882   | 0.913   | 0.931         |0.769         |
| BLEU4      | 0.670  | 0.606   | 0.762   | 0.848   | 0.804         |0.583         |
| BLEU5      | 0.489  | 0.437   | 0.618   | 0.780   | 0.746         |0.408         |

More detailed benchmark settings and evaluation results are provided [here](docs/evaluation.md).

## Reference

@article{zhu2018texygen,<br>
&nbsp;&nbsp;&nbsp;&nbsp;  title={Texygen: A Benchmarking Platform for Text Generation Models},<br>
&nbsp;&nbsp;&nbsp;&nbsp;  author={Zhu, Yaoming and Lu, Sidi and Zheng, Lei and Guo, Jiaxian and Zhang, Weinan and Wang, Jun and Yu, Yong},<br>
&nbsp;&nbsp;&nbsp;&nbsp;  journal={arXiv preprint arXiv:1802.01886},<br>
&nbsp;&nbsp;&nbsp;&nbsp;  year={2018}<br>
}

