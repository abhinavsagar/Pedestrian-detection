# Pedestrian-detection
Pedestrian Detection using Non Maximum Suppression

Check out the corresponding medium blog post [https://towardsdatascience.com/pedestrian-detection-using-non-maximum-suppression-b55b89cefc6](https://towardsdatascience.com/pedestrian-detection-using-non-maximum-suppression-b55b89cefc6).

## Environment and tools

1. scikit-learn
2. scikit-Image
3. numpy
4. opencv
5. nms
6. argparse

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

1. https://arxiv.org/abs/1904.03629

2. https://www.frontiersin.org/articles/10.3389/fnbot.2018.00064/full

3. https://www.cs.cmu.edu/~efros/courses/LBMV07/Papers/leibe-cvpr-05.pdf

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

## Contacts

If you want to keep updated with my latest articles and projects follow me on Medium. These are some of my contacts details:

1. [Personal Website](https://abhinavsagar.github.io/)
2. [Linkedin](https://in.linkedin.com/in/abhinavsagar4)
3. [Medium](https://medium.com/@abhinav.sagar)
4. [GitHub](https://github.com/abhinavsagar)
5. [Kaggle](https://www.kaggle.com/abhinavsagar)







