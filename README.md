# deeplearning

	Purpose?
Train CIFAR10 with PyTorch, and upgrade accuracy on CIFAR-10

	Used Model?
MobileNetV2

	Abstract
The aim of this research report is to develop deep neural architecture to obtain high accuracy for CIFAR10 dataset. 

	Prerequisites
Python 3.6+
PyTorch 1.0+

	Modifications and Results?
1.	Original
Result? 92.560%


2.	Add random rotation as 10.
Transforms.RandomRotation(10).
Result? 92.480%

3.	Add random rotation as 11
Transforms.RandomRotation(11).
Result? 92.610

4.	Add random rotation as 9
Transforms.RandomRotation(9).
Result? 92.660

5.	Add the gaussian blur
Transforms.GaussianBlur(kernel_size=3),
Result? 91.890

6. Resize the image
    transforms.Resize((32,32)),
Result? 92.790

7. Add random rotation as 12
Transforms.RandomRotation(12).
Result? 92.780

8. Edit the default value as 0.01
pareser.add_argument('--lr', default=0.01, type=float, help='learning rate')
Result? 93.750




