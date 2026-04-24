# ProVioNet
PreVioNet: A Dual-Backbone Temporal Attention Fusion Network for Violence Forecasting in Videos
Globally, there is growing concern about violence in public areas; however, current automated
monitoring systems only detect violence after it has already taken place. In order to bridge the gap between
reactive detection and proactive prevention, this work introduces the problem of pre-violence prediction,
which involves determining whether a video clip taken immediately prior to a physical altercation (the
escalation phase) differs from typical non-violent behavior. This paper introduces PreVioNet, a dualbackbone
temporal attention fusion network designed to predict violence in security footage. In order to
capture hierarchical semantic information and fine-grained postural patterns, the architecture integrates
two complimentary spatial feature extractors, Xception and ResNet101, both of which were pretrained on
ImageNet. The concatenated backbone outputs are projected into a lower-dimensional space using a feature
fusion layer, and then a bidirectional LSTM is used for temporal modeling. After that, a temporal attention
mechanism learns which temporal segments are most discriminative for escalation detection by dynamically
fusing the hidden states. This work selected 179 videos (95 pre-fight and 84 normal activity clips) from the
NTU CCTV-Fights archive to aid in this effort. PreVioNet attains a mean accuracy of 93.32% ± 2.81% using
5-fold stratified cross-validation. For pre-fight data, the model has perfect recall (1.0) and best fold accuracy
(97.14%), indicating a 2.70% improvement as compared to the second-best model. PreVioNet outperforms
several baseline methods, including hybrid multistream architectures (94.29%) and MobileNetV3+Positional
Encoder+ViT (94.44%). According to attention-based interpretability analysis, the model only focuses on
highly informative frames and busy spatial locations during violent incidents. It gives equal emphasis to
every frame in regular sequences for normal activity. These findings demonstrate that violence is not only
predictable but also very likely to occur. This makes it possible to go from reactive surveillance to proactive
action.
INDEX T
