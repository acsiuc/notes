# INTERVIEW QUESTIONS

## What happens if the learning rate is too high? What happens if it is too low?

If the learning rate is too low, then the steps toward the minimum might be too low and the network might never converge or it would get stuck at a local minimum, if the learning rate is too high, then there is the possibility that the learning rate would also never get to the minimum we want since the steps are too big

Some fixex would be a learning rate scheduler, which would consist in lowering the rate over time, or adaptive optimizers like Adam

## What is the difference between a batch, an epoch, and an iteration in training?

A batch is a grouping of multiple samples from the dataset, like 32 imags maybe, an epoch is one full pass over the whole dataset, and an iteration is a loss optimization over a batch, which updates the weights and the loss changes as a result (forward pass, loss, backward pass, update)