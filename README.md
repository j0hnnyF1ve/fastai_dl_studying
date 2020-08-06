# fastai_dl_studying
My personal repo on notes and papers that helped with studying DL, fast.ai etc

## Tips

- Watch all lectures three times
  - First time, watch at a comfortable speed (1-1.5x)
  - Subsequent times, can watch at faster speeds, and replay/focus on parts that you didn't understand the first time
- Write more code once you start understanding things a little
  - Implementing 

## Important Concepts described in Papers

### Dropout

[Dropout: A Simple Way to Prevent Neural Networks from
Overfitting](https://www.cs.toronto.edu/~hinton/absps/JMLRdropout.pdf)
- Reading difficulty level: 4/10 (** double check this value)
- Main Intuition(s): 
  - Dropout has a regularizing effect on a wide variety of architectures (in other words, it operates generally)
  - It prevents overfitting by making the network more sparse, and preventing nodes from codepending on one another (** double check this claim)
- Useful Concepts to know:
  - Bernoulli Distribution
  - RBMs (Restricted Bolzmann Machines)
- Notes:
  - A great paper describing how dropout works
  - Fairly easy read, not that math heavy
  - Stochasticity of dropout prevents overfitting, with the cost being training time
- Drawbacks:
  - Adding dropouts can increase training time (typically 2-3 times longer for standard neural network)
    - Parameter updates are very noisy
    - Each training case is basically training a different architecture
    - Gradients being computed aren't gradients of the final architecture
