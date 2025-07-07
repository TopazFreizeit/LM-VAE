# Information Theory & LMs
## Reichman Universty
#### Students: Omri Drori & Topaz Freizeit
#### Guided by Dr. Alon Kipnis

Variational Autoencoders (VAEs) are powerful generative models that compress high-dimensional data into a structured, lower-dimensional latent space. This architecture features a probabilistic encoder to map data into this latent space and a probabilistic decoder to reconstruct the data from it. Training is governed by the Evidence Lower Bound (ELBO) objective, which balances the trade-off between reconstruction accuracy and a regularization term that organizes the latent space. In Natural Language Processing, VAEs can model holistic sentence properties like topic and style, with modern systems using LLMs like BERT as an encoder and GPT-2 as a decoder.

The VAE's training objective can be framed by Rate-Distortion theory, which formalizes the trade-off between compression (Rate) and reconstruction quality (Distortion). A major challenge is "posterior collapse," where the latent code becomes uninformative because the model overly prioritizes compression, effectively ignoring the encoder's output. By creating an "information bottleneck" through this trade-off, VAEs can be encouraged to learn disentangled representations. Advanced VAEs aim to improve this disentanglement by directly minimizing the statistical dependence between latent dimensions, resulting in a more interpretable and controllable generative process.

The attached slides present the theory of VAEs, and the notebook presents the connection between VAEs and text generation.