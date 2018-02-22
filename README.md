<h1>DiversityNet</h1>

DiversityNet is a benchmarking platform to support research on molecule generation models. DiversityNet is not only implementing a majority of molecule generation models, but is also covering a set of metrics that evaluate the diversity and the quality of the generated molecules. The DiversityNet platform could help standardize the research on molecule generation and facilitate the sharing of fine-tuned open-source implementations among researchers and practitioners.  As a consequence, this would help in improving the reproductivity and reliability of future research work in molecule generation.

For more details, please refer to our Authorea paper: [DiversityNet: a collaborative benchmark for generative AI models in chemistry](https://www.authorea.com/users/226673/articles/285209-diversitynet-a-collaborative-benchmark-for-generative-ai-models-in-chemistry) .

Should you have any questions and enquiries, please feel free to contact us on [Telegram](https://t.me/joinchat/Go4mTw0drJBrCdal0JWu1g) or otherwise Mostapha Benhenda (mostaphabenhenda [AT] gmail.com).

## Requirement
We suggest you run the platform under Python 3.6+ with following libs:
* **TensorFlow 1.3.0**
* Numpy 1.12.1
* Scipy 0.19.0
* NLTK 3.2.3
* CUDA 7.5+ (Suggested for GPU speed up, not compulsory)    

* Rdkit (to do)

Or just type `pip install -r requirements.txt` in your terminal.

## Implemented Metrics

* Internal diversity (see self-diversity): (https://github.com/mostafachatillon/ChemGAN-challenge/blob/b70d0b2c1efc00ecade3fde1896751876a89e9ec/model/mol_metrics_new2.py#L277) 

To do:
* Nearest-Neighbor diversity
* Entropy
* Earth mover
* Frechet ChemblNet Distance (contact @gklambauer (https://github.com/gklambauer) )
* ...



## Implemented Models and Original Papers

* See the list here: (https://medium.com/the-ai-lab/diversitynet-a-collaborative-benchmark-for-generative-ai-models-in-chemistry-f1b9cc669cba#27e5)

* **SeqGAN** -  [SeqGAN: Sequence Generative Adversarial Nets with Policy Gradient](https://arxiv.org/abs/1609.05473)

* **MaliGAN** - [Maximum-Likelihood Augmented Discrete Generative Adversarial Networks](https://arxiv.org/abs/1702.07983)

* **RankGAN** - [Adversarial ranking for language generation](http://papers.nips.cc/paper/6908-adversarial-ranking-for-language-generation)

* **LeakGAN** - [Long Text Generation via Adversarial Training with Leaked Information](https://arxiv.org/abs/1709.08624)

* **TextGAN** - [Adversarial Feature Matching for Text Generation](https://arxiv.org/abs/1706.03850)
 
* **GSGAN** - [GANS for Sequences of Discrete Elements with the Gumbel-softmax Distribution](https://arxiv.org/abs/1611.04051)


## Get Started

```bash
git clone https://github.com/startcrowd/DiversityNet.git
cd Texygen
# run SeqGAN with default setting
python3 main.py
```
More detailed documentation for the platform and code setup is provided [here](docs/doc.md).


## Evaluation Results

Coming soon 
## Reference

@article{diversitynet2018,<br>
&nbsp;&nbsp;&nbsp;&nbsp;  title={DiversityNet: a collaborative benchmark for generative AI models in chemistry},<br>
&nbsp;&nbsp;&nbsp;&nbsp;  author={Mostapha Benhenda and Esben Jannik Bjerrum,...},<br>
&nbsp;&nbsp;&nbsp;&nbsp;  journal={Authorea preprint},<br>
&nbsp;&nbsp;&nbsp;&nbsp;  year={2018}<br>
&nbsp;&nbsp;&nbsp;&nbsp;  url={https://www.authorea.com/users/226673/articles/285209-diversitynet-a-collaborative-benchmark-for-generative-ai-models-in-chemistry}<br>
}

This code is based on Texygen (https://github.com/geek-ai/Texygen). Many thanks to [Geek.AI](http://geek.ai/)
