# Pedestrian-detection
Pedestrian detection using Non Maximum Suppression.

## If this repository helps you in anyway, show your love :heart: by putting a :star: on this project :v:

Check out the corresponding medium blog post [https://towardsdatascience.com/pedestrian-detection-using-non-maximum-suppression-b55b89cefc6](https://towardsdatascience.com/pedestrian-detection-using-non-maximum-suppression-b55b89cefc6).

## Environment and tools

1. scikit-learn
2. scikit-Image
3. numpy
4. opencv
5. nms
6. argparse

## Data

I downloaded the images from [here](https://unsplash.com/search/photos/pedestrians).
Then I compressed the image to 300 by 200 size and used these images as test images
for this project.

## Non Maximum Suppression

History of Oriented Gradients(HOG) combined with Support Vector Machines(SVM) have
been pretty successful for detecting objects in images but the problem with those
algorithms is that they detect multiple bounding boxes surrounding the objects in
the image. Hence they are not applicable in our case that is detecting pedestrians 
on crowded roads. Here's where Non maximum suppression(NMS) comes to rescue to better
refine the bounding boxes given by detectors. In this algorithm we propose
additional penalties to produce more compact bounding boxes and thus become less
sensitive to the threshold of NMS. The ideal solution for crowds under their pipelines
with greedy NMS is to set a high threshold to preserve highly overlapped objects and
predict very compact detection boxes for all instances to reduce false positives.

## To execute

`python run.py -i sample_images/p2.jpg`

## Results

![](output.jpg)

## References

1. https://www.cs.cmu.edu/~efros/courses/LBMV07/Papers/leibe-cvpr-05.pdf

2. https://www.frontiersin.org/articles/10.3389/fnbot.2018.00064/full

3. https://arxiv.org/abs/1904.03629

4. https://www.vision.ee.ethz.ch/publications/papers/proceedings/eth_biwi_01126.pdf

## Citing

```
@misc{Abhinav:2019,
  Author = {Abhinav Sagar},
  Title = {Pedestrian detection using Non Maximum Suppression},
  Year = {2019},
  Publisher = {GitHub},
  Journal = {GitHub repository},
  Howpublished = {\url{https://github.com/abhinavsagar/Pedestrian-detection}}
}
```







