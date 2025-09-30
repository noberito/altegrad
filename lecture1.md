# Word Embeddings, Attention, NLP tasks and metrics

## Representation Learning for Text

### Representing words

For one-hot vectors, the matrices represent the appearance of each word (lines) in the vocabulary in the documents (columns)

For distributional vectors, it is the frequency for each word of the vocabulary (line) to be present with a word of the vocabulary (columns).

We define the similarity for two words in the vocabulary as:

$$sin(d_j, d_m) = cos(\theta)$$

where $\theta$ is the angle between the vector representation of the 2 words.

$$ \frac{\vec{w_i}.\vec{w_l}}{\lvert \vec{w_i} \rvert.\lvert \vec{w_l} \rvert}$$

Problem with one-hot vector and distributional vector: sparse.

### SVD (Singular Value Decomposition) word embeddings

Methodology for the example in the slides: 
* From a one-hot vector, perform SVD
* Keep the 2 largest singular values
* Perform $U_kL{V^T}_k$ 
* Get the word embedding

A query is a vector of in the vocabulary coordonates of the words in the query.

See the calculation again.

### Word2Vec