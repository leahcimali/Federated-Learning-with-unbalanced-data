# Federated-Learning-Unbalancing

Federated learning (FL) is a recent decentralized approach used in machine learning on a
wide range of devices which respect privacy and security on local devices by decentralized
training on each client and averaging the model.

However, distribution, imbalance, number of clients and quantity of data in the client side
lead to a whole share of challenges for model performance. While literature tackled a big
number of challenges for non-IID (non-independent and identically distributed) data, the
issue of class imbalance has not been addressed enough.

Federated learning techniques nowaday are working a bit like a black box as the training
data are only partially observable to either clients or server side. In particular, FL training is
executed by exchanging gradients in an encrypted form so the usual method to tackle class
imbalance in centralized machine learning does not perform well here and may be quite hard
to put in place effeciently.

As we said, since how the training and the model averaging work are kind of like a black
box, finding how exactly different cases of unbalancing are going to impact our model
averaging is quite interesting. During this internship, we tried to observe how the different
cases of unbalancing are going to impact our global model performance. We want to
compare the effect of local unbalancing which corresponds to unbalanced data on each
node but with global balancing, global unbalancing which correspond to data which are
locally and globally unbalanced and finally have a look at the effect of missing values on
local nodes.

Our experiment will be tested on the MNIST dataset which has been quite heavily used as a
benchmark in federated learning problems and algorithms. All experiments will be tested
using Pytorch and we will compare results as centralized learning with federated learning
and compare results in different cases of imbalance.
