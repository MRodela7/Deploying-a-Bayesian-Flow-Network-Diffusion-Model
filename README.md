# Deploying-a-Bayesian-Flow-Network-Diffusion-Model
Applying a BFN diffusion model (with a UNet base model) on molecule smile embedding to understand the control of finding potential drug candidates
by conditioning on logP values (which dictate the likelihood of an embedding vector to be a drug. 
A linear regression model was trained using the embedding vectors and then the bfn model was used to synthesize potential drugs. A comparison was drawn among the synthesized drugs and the original ones. The syntehsized drugs were then used to predict it's corresponding logP values. Finally, the bfn model was once more trained using conditioned embedding vectors, based on the logP values, and new logP was gathered from the conditioned synthesized ones and a comparison was drawn.
However, due to compute power, the trainning sample size was significantly small, and so was the step size in generating the new smile embeddings.
