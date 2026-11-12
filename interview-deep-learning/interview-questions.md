# INTERVIEW QUESTIONS

## What happens if the learning rate is too high? What happens if it is too low?

If the learning rate is too low, then the steps toward the minimum might be too low and the network might never converge or it would get stuck at a local minimum, if the learning rate is too high, then there is the possibility that the learning rate would also never get to the minimum we want since the steps are too big

Some fixex would be a learning rate scheduler, which would consist in lowering the rate over time, or adaptive optimizers like Adam

## What is the difference between a batch, an epoch, and an iteration in training?

A batch is a grouping of multiple samples from the dataset, like 32 imags maybe, an epoch is one full pass over the whole dataset, and an iteration is a loss optimization over a batch, which updates the weights and the loss changes as a result (forward pass, loss, backward pass, update)

## Your model trains well with batch size 32. You change it to 1024 and accuracy gets worse. Give one possible reason

One possible reason would be that the dataset is too small for a batch size of 1024, which would mean less updates per epoch, resulting in a higher loss than expected

## What is a CNN (Convolutional Neural Network)

A convolutional network is a type of neural network that is used for data  with a grid structure, a normal network treats every pixel as a separate input, a CNN looks at small regions of images and slides small filters over the image

## In a CNN, what does a convolutional layer do to an image?

It slides small filters(kernels) over parts of that image and tries to find patterns like edges, multiplying each filter value by the pixel under 

## What is a pooling layer, and what is max pooling?

A pooling layer makes the feature map smaller. It slides a small window over the map and replaces each window with one number. Max pooling: the one number is the largest value in the window, pooling reduces computation and keeps the strongest response, so the model still knows a pattern is present

## Max pooling throws away 3 out of every 4 values. Why is this usually acceptable for image recognition?

The high value already tells us the pattern is present, for recognition we need to know that the pattern exists in the region, not its exact pixel, the 3 discarded values are weaker responses and add little information