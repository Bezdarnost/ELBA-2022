Hello, everyone. My name is Aman Urumbekov. 
I am a student of KSTU, I am studying in the first year at the Faculty of Applied Mathematics and Computer Science / Analysis and Data Processing. 
Also I am Computer Vision Engineer and Competitive Programmer. Recently, I made it to the quarterfinals of ICPC. 

First, let's understand what deep learning is. 
Deep learning is a type of machine learning based on artificial neural networks. 
The learning process is called deep learning because the structure of artificial neural networks consists of several input, 
output, and hidden layers. Each layer contains units that transform input data into information 
that the next layer can use for a particular prediction task. Because of this structure, the computer can learn with its own data processing.
	
The features of deep learning:
	
-The Number of Data Points:
-It is necessary to use large amounts of training data to create predictions.
	
-Hardware Dependecies:
-Requires powerful machine, preferably with GPU: DL performs a significant amiunt of matrix multipliction.
	
-Execution Time:
-Up to weeks. Neural Netowrk need to compute a significant number of weights.
	
And now I want to list some Deep Learning applications.
-Image Recognition.
-Automatic Language Translation.
-Medical Diagnosis.
-Stock Market Trading.
-Virtual Personal Assistant.
-Speech Recognition.
	
What do the representations learned by a deep learning algorithm look like? Let’s
examine how a network several layers deep transforms an image of a
digit in order to recognize what digit it is.

As you can see in image, the network transforms the digit image into representations that are increasingly different from the original image and increasingly informative about the final result. You can think of a deep network as a multistage information-
distillation process, where information goes through successive filters and comes out
increasingly purified (that is, useful with regard to some task).

So that’s what deep learning is, technically: a multistage way to learn data representa-
tions. It’s a simple idea—but, as it turns out, very simple mechanisms, sufficiently
scaled, can end up looking like magic.
	
	
	
Now let's get to the main part.
Today I have prepared some neural networks for a visual comparison of some optimization algorithms.
First, let me tell you about my computer, on which I have trained neural networks.
My system configuration is:
-32 GB of RAM.	
-GPU is RTX 3060 with 12 GB of VRAM.
-CPU is AMD Ryzen 5 3600.
	
And I used a programming language like Python as a tool. 
I also used Pytorch library to create neural networks and train them, and for visualization I used MatPlotLib.
	
I used a dataset of 4,000 photos of cats and 4,000 photos of dogs for training. 
And at the end I tested the neural network on 2,000 photos of cats and dogs.
	
In this block I import all libraries.
	
In this block I prepare data.
	
This is an example of images from dataset. 
	
In this block I build my Neural Network. I used the main body from an existing neural network. 
It's a VGG-19. This neural network was developed at the University of Oxford. 
I added my own classifier at the end, to improve the accuracy of the answers. 
In this model I used the optimizer Adam. This method of creating neural networks is called transfer learning. 
This method is very popular now, because thanks to it you can use not so much data and get excellent accuracy of predictions.
	
This is a detailed description of my neural network, with each layer of neurons. 
There are about 20 million parameters in this neural network.
	
And here is the end of all development, a block with neural network training in 5 epochs. 
You can see how much time was spent training.
	
And here is our graph of prediction accuracy on test data after each training epoch.
	
Then I did the same thing twice more, but using different optimizers.
	
And finally in this graph we can see a clear comparison of three different optimizers. 
	
Adam, Stochastic Gredient Descent and RMSPropagation. My personal favorite is the optimizer Adam, 
because it is very fast and powerful. Let me tell you a little bit about it.
	
Adam

Adaptive Moment Estimation (Adam) is the optimizer that performs the best on average. 
Taking a big step forward from the SGD algorithm to explain Adam does require some explanation of some clever techniques 
from other algorithms adopted in Adam, as well as the unique approaches Adam brings.

Adam uses Momentum and Adaptive Learning Rates to converge faster. We have already explored what Momentum means, 
now we are going to explore what adaptive learning rates means.
	
I have prepared a small animation of the work of various other optimizers. Optimizers help, 
as quickly as possible to come to a minimum of losses. The smaller our losses, the better the accuracy of the neural network model. 
This concludes my report, thank you all for your attention, does anyone have any questions?
