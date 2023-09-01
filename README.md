# Machine-Unlearning
<br/>

The function "unlearn" is an algorithm I wrote in which the weights of the retrained model are approxiamated by fine tuning the weights of the pretrained model. It tries to reverse the influence of the training examples in the forget set and gain more epochs training on the elements of the retain set. It achieves almost perfect forgetting quality, and retains much of the function of the pretrained model.


The pretrained, retrained, and fine-tuned models were subject to a Membership Inference Attack and the accuracies of the attacks were 0.58, 0.50, and 0.50 respectively, strongly implying that the fine-tuned model is nearly invulnerable to MIAs. The official criteria for evaluation is yet to be released but it works similarly to this one.

The retrained model has the following accuracies on the relevant datasets:

Retain set accuracy: 99.5%

Test set accuracy: 88.2%

Forget set accuracy: 88.0%

And here are the results for the fine-tuned model:
Retain set accuracy: 99.0%

Test set accuracy: 83.6%

Forget set accuracy: 83.2%


Unfortunately the fine tuned-model suffers slightly in terms of its accuracy on the test and forget set, but I hope this gap will close in time once I start working on this algorithm with members of Neurotechnology@Berkeley. This is one of our candidate algorithms for our submission to the NeruIPS 2023 Machine Unlearning Challenge.

