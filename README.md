# noisyphotonicDNNs
Training techniques for improving the robustness of photonic analog deep neural networks

Optical computing is promising for edge inferencing applications due to the ability to perform energy-efficient linear matrix multiply operations at ultra-high speeds and low latencies. However, since optical computation is analog by nature, noise in the circuitry or input/output plays a critical role in determining the accuracy of the system. One prominent technique to counter this involves adding noise during training ("standard Gaussian noise injection") to closely mimic the inferencing analog hardware. Here, we show how distillation can be used in combination with standard Gaussian noise injection to improve the accuracies of analog photonic inferencing hardware and make them more robust. This has been previously shown for memristor-based hardware architectures [1].

As a result, we have three different notebook files. One is the baseline, where the training is done without noise and the inferencing is also on clean hardware. There is the option of adding noise only during inferencing and checking the detrimental effect of noise on test accuracies. The other two notebook files include the codes for the standard Gaussian injection technique and the distilled Gaussian technique. We add the noise to the activations which is in contrast to the memristor-based approaches where the noise is added to the weights. This has to do with the noise sources present in photonic deep neural networks. 

 References:
 1. C. Zhou, P. Kadambi, M. Mattina, and P. N. Whatmough, “Noisy Machines: Understanding Noisy Neural Networks and Enhancing Robustness to Analog Hardware Errors Using Distillation,” arXiv:2001.04974, Jan. 2020
