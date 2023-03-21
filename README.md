<p align="center">
	<img src="logo.png" alt="logo frechet" width="600"/>
</p>

# Fréchet Statistics-based Network Change Detection
Our proposed approach is a Fréchet statistics-based method that utilizes binary segmentation for detecting multiple change points in dynamic networks. Please find the details in [Fréchet Statistics Based Change Point Detection in Dynamic Social Networks](http://128.84.21.203/abs/2303.10753) [1].

By leveraging the Fréchet mean and variance, our method is able to effectively capture changes in the network structure over time, while binary segmentation along with an incremental Fréchet mean and variance computation enable efficient detection of multiple change points. 

We also provide a re-implementation of the baseline LAD (KDD' 20) [2] method.

## Enron email dataset
- Download the text file (`datasets/execs.email.linesnum.txt`) from [a processed version](https://www.cis.jhu.edu/~parky/Enron/), where each email is represented as a tuple containing the email's timestamp, sender, and recipient.
- Run the jupyter notebook (`preprocessing_Enron.ipynb`) to extract weekly email networks from the text file. The notebook will construct a list of networks, each representing a one-week period, and then save the results as a Python pickle file (`datasets/enron_weekly.pkl`).


## References
[1]
```
@misc{luo2023frchet,
    title={Fréchet Statistics Based Change Point Detection in Dynamic Social Networks},
    author={Rui Luo and Vikram Krishnamurthy},
    year={2023},
    eprint={2303.10753},
    archivePrefix={arXiv},
    primaryClass={cs.SI}
}
```
[2] 
```
@inproceedings{huang2020laplacian,
  title={Laplacian change point detection for dynamic graphs},
  author={Huang, Shenyang and Hitti, Yasmeen and Rabusseau, Guillaume and Rabbany, Reihaneh},
  booktitle={Proceedings of the 26th ACM SIGKDD International Conference on Knowledge Discovery \& Data Mining},
  pages={349--358},
  year={2020}
}
```
