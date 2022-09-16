The data and code in this repository are supplementary materials to the paper
### Introducing Encoder-Decoder Relation between Cellular Automata to Uncover their Computational Structure
by Barbora Hudcová, Tomáš Mikolov, and Stefano Nichele

In the paper, we introduce the relation between cellular automata called the enc-dec simulation. Informally we say that $\mathrm{ca}_1$ can be enc-dec simulated by $\mathrm{ca}_2$ if some-larger scale dynamics of $\mathrm{ca}_2$ contains the dynamics of $\mathrm{ca}_1$.

##### Search Methods
In the Jupyter notebook "enc_dec_sim_search_simple.ipynb" you can find the basic algorithm we used for searching for relations between elementary cellular automata. 

##### Results
The "eca_relations_database.json" file contain the json dictionary of all the 548 relations we found for elementary cellular automata. Suppose we have a relation showing that $\mathrm{ca}_1$ can be simulated by $\mathrm{ca}_2$ with an encoder of size $k$. The relation is stored in the database in the following manner:

it is identified by the key " $\mathrm{ca}_{1}$ _ $\mathrm{ca}_2$" and its value is:

{"cell_size": $k$, "enc": $\[enc(0)$, $enc(1)\]$, "dec": $\[ dec^{-1}(0)$, $dec^{-1}(1) \]$}
