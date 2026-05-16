**Part 2: Computer Vision Problem Formulation and CNN Prototype**



***Task 1: Problem Identification***
The computer vision problem that we have detected is "image classification problem".

**Reason**: We have a dataset where each image is labeled with one of four categories such as normal, scratch, dent and stain. This means that every picture belongs to exactly one class. In image classification, the computer looks at a whole picture and decides which category it belongs to.

Here, the categories are types of car surface conditions (normal, scratch, dent, stain). We are not trying to find where the scratch or dent is (that would be object detection or segmentation). We are simply asking: “Is this picture normal, scratched, dented, or stained?” So it is "**Image Classification**".



\-------------------------------------------------------------------------------------------------

***Task 6: CNN Concept Explanation***

**Question - What is convolution?**

**Answer** 

* Convolution is a mathematical operation that acts as a filter, sliding across an input (like an image) to automatically detect spatial features—such as edges, corners, or textures—by calculating dot products between the filter and local pixel patches, producing a "feature map". 
* It is how the network extracts features from images — edges, textures, shapes, and eventually complex objects.
* It allows models to identify patterns regardless of their position**.**



**Question - Why is pooling used?**

**Answer** 

Pooling is a down sampling operation that reduces the spatial dimensions of feature maps while retaining the most important information. It serves three purposes:

* Reduces computation — smaller feature maps mean fewer calculations in subsequent layers.
* Reduces overfitting — fewer parameters and a more abstract representation help the model generalize.
* Provides translation invariance — small shifts in the input produce the same pooled output.



**Question - Why is ReLU commonly used in CNNs?**

**Answer** 

Three reasons ReLU is preferred:

* No vanishing gradient for positive values: The gradient is always 1 for positive inputs. This means gradients flow freely through deep networks during backpropagation, enabling effective training of networks with many layers.
* Computationally cheap: A simple comparison (x>0?) is far faster than computing exponentials (e^(-x)). In a CNN processing millions of values per forward pass, this efficiency adds up.
* Sparsity: Negative values are zeroed out, creating sparse activations — many neurons output zero. This helps the network focus on the most relevant features and acts as a form of implicit regularization.



**Question - Why are CNNs better than regular feed forward networks for image data?**

**Answer** 

* Regular feed forward networks treat every pixel separately, which is too much information.
* CNNs use convolution filters to focus on local patterns such as edges, shapes, textures. This makes them smarter and more efficient for images. It’s like comparing a person who memorizes every grain of sand on a beach (feed forward) and a person who notices “this is a beach with waves and shells” (CNN).



\-------------------------------------------------------------------------------------------------



**Task 7: Business Use Case Mapping**

Imagine there is a car factory where thousands of vehicles roll off the assembly line every single day. While human inspectors usually check for scratches, dents, and stains on car surfaces; however, this is a slow and tiring process which also has a scope of error



**With CNN solutioning:**

* Image classification can be incorporated for automatic detection of car surface. It can help identify normal, scratched, dented, or stained surface.
* Cameras can be installed with the production line capturing images of each car.
* With this approach CNN model will be able to classify defects in real time.
* If a defect is identified, the system will alerts workers to fix it before the car is shipped.



**Benefits for Manufacturing**

* Faster inspections as CNNs processes images much faster than humans.
* Consistency as there is no fatigue or bias eliminating human error. 
* This will be cost savings as early defect detection reduces rework and warranty claims.
* Scalable as it works across multiple factories and production lines.







