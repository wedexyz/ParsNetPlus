# ParsNetPlus
ParsNet++: Autonomous Deep Quality Classification with Weak Supervision

# Abstract
An autonomous quality monitoring approach is desired in practise since it allows to relieve operator's intervention in inspecting the product quality. Such approach should be not only data-driven but also be capable of handling various operational uncertainties of manufacturing processes including streaming nature of sensory data, variations of machine parameters. While pioneering works have been proposed in the domain of online condition monitoring problem featuring one-pass learning mode and self-evolving characteristic to combat rapidly changing environments of manufacturing conditions, such approach deserves further exploration to actualize a truly autonomous quality monitoring method. The underlying reason pertains to the fact of expensive labelling cost often calling for manual inspection. Parsimonious Network++ (ParsNet++) is proposed as a self-organizing deep learning approach to cope with the online product quality monitoring problem with weak supervision. ParsNet++ is capable of dealing with random access of ground truth as well as infinitely delayed access of ground truth in realm of online product quality classification while having a self-evolving property rendering it well-suited to handle varieties of process changes. Furthermore, it is capable of performing automatic feature engineering mechanism where the 1-D CNN is integrated as a feature extraction layer processing multivariate time-series data samples of sensors thereby improving its predictive performance without manual feature extraction step as well as handling the many-to-one label relationship. Our experiment is carried out in the injection molding process and in the industrial transfer molding process from our own project. It demonstrates that ParsNet++ achieves state-of-the art accuracy even compared to fully supervised techniques.  

# Requirements
The current version of the code has been tested with:
* 'pytorch 1.3.1'
* 'torchvision 0.4.2'

# Running the experiment
All experiments with injection molding dataset can be run with 'NextBatchPredict.py', 'CurrentBatchPredict.py', 'InfiniteDelayNext.py', 'InfiniteDelay.py', and 'NextBatchPredict_proportion.py'. The link between individual experiments and scripts are listed as follow:
Sporadic access next batch prediction -- 'NextBatchPredict.py'
Sporadic access current batch prediction -- 'CurrentBatchPredict.py'
Infinite delay next batch prediction -- 'InfiniteDelayNext.py'
Infinite delay current batch prediction -- 'InfiniteDelay.py'
Effect of different label proportion -- 'NextBatchPredict_proportion.py'
A comparison of classification performance on ParsNet++ included in the paper can be run with 'plot-cur.ipynb' and 'plot-next.ipynb' (Figure 4).
