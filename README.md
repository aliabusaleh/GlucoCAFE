# GlucoCAFE
**NOTE** Work is submitted to conferances

### summary 
we proposed a new deep learning architecture to mitigate the preprocessing assumptions, and perform context-aware preprocessing, building a latent space for the data, leading to generalized model, with a longer prediction horizon. We also introduce a probability-based event labeling, considering a window of data to capture physiological responses to certain events.

The model architecture relies on a variational auto-encoder (VAE) to produce a preprocessing latent space, and a recurrent VAE to preserve the temporal dynamics of the data, followed by a transformer head to perform a long/short term predictions with zero-shot-learning setup. On the other hand, the event detection relies on capturing analysing within a window of 3-hours as probability rather than a static values.

We demonstrate the effectiveness of such an architecture on telemonitoring data to forecast glucose-level of diabetic patients. 
We utilized two datasets, OhIoT1DM dataset (6 patients, total of 65K readings, 8-weeks study period), and private dataset (12,827 patients, total of 2.3 billion readings, 5-years study period).

Our results show an improvement in terms of accuracy with respect of existing state-of-the-art methods and architectures on both mathematical and clinical metrics.