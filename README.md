<img src="logo.png" alt="logo frechet" width="640"/>

# network-change-detection
Fréchet mean based method (quadratic approximation of the Laplacian entropy), re-implementation of the LAD (KDD' 20) method

## Enron email dataset
- Download the text file (`datasets/execs.email.linesnum.txt`) from [a processed version](https://www.cis.jhu.edu/~parky/Enron/), where each email is represented as a tuple containing the email's timestamp, sender, and recipient.
- Run the jupyter notebook (`preprocessing_Enron.ipynb`) to extract biweekly email networks from the text file. The notebook will construct a list of networks, each representing a two-week period, and then save the results as a Python pickle file (`enron_biweekly.pkl`).