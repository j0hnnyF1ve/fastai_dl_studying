# fastai_dl_studying
My personal repo on notes and papers that helped with studying DL, fast.ai etc

## Course Notes for fastai course 2019
### Part 1

TODO

### Part 2

By Medium user [@lankinen](https://medium.com/@lankinen)
- [Lesson 8](https://medium.com/@lankinen/fast-ai-lesson-8-notes-part-2-v3-8965a6532f51)
- [Lesson 9](https://medium.com/@lankinen/fast-ai-lesson-9-notes-part-2-v3-ca046a1a62ef)
- [Lesson 10](https://medium.com/@lankinen/fast-ai-lesson-10-notes-part-2-v3-aa733216b70d)
- [Lesson 11](https://medium.com/@lankinen/fast-ai-lesson-11-notes-part-2-v3-6d28e17509f4)
- [Lesson 12](https://medium.com/@lankinen/fast-ai-lesson-12-notes-part-2-v3-dd53bec89c0b)
- [Lesson 13](https://medium.com/@lankinen/fast-ai-lesson-13-notes-part-2-v3-2d62ef11d2db)
- [Lesson 14](https://medium.com/@lankinen/fast-ai-lesson-14-notes-part-2-v3-be4667394295)


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

### Batch Normalization
[arXiv:1502.03167v3  [cs.LG]  2 Mar 2015 Batch Normalization: Accelerating Deep Network Training by Reducing Internal Covariate Shift](https://arxiv.org/abs/1502.03167)
- Reading difficulty level: 6/10, some math, 
- Main Intuition(s): <todo>
- Useful Concepts to know: <todo>
- Notes:
  - As a SOTA image classification model, BN achieves same accuracy with 14 fewer steps, and beats original model by significant margin
  - Gradient of a mini-batch's loss is an estimate of gradient over the training set, quality improves as batch size increases
  - BN reduces dependence of gradient on scale of parameters and/or initial values
    - Leads to usage of higher learning rates w/o risk of divergence
  - BN regularizes the model, reduces need for Dropout


### Article Template
[name](link)
- Reading difficulty level: 
- Main Intuition(s):
- Useful Concepts to know:
- Notes:

