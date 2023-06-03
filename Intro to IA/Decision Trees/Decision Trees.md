Another classifier but this one is easy to read by humans. This one works by mapping information into a tree like decision structure. 
![[DT.example1.excalidraw.svg]]

We can intuivelly determine where to split a dataset to separate the datapoints efficiently, but how do w translate that into an algorithm?

## Entropy
We use entropy to decide where to split the data. The informal definition of entropy would be '*the measure of impurity in a bunch of examples*' or the inverse of the purity of a set.
![[DT.example2.excalidraw.svg]]
Intuitively a dataset where all observations are evenly split will have entropy 1, and a dataset where all points are of the same class will have entropy 0.
The formula for entropy is as follows:
$$
entropy =  \sum\limits_{i}{-Pi\cdot \log_{2}Pi}
$$
Note: Some sources use log of base 10, or ln. This affects the maximum possible entropy depending on the formula. For log of base 2 the maximum entropy would be 1, as mentioned after the example above.

### Calulating entropy
![[DT.example3.excalidraw.svg]]

So we can calculate the entropy of a node, how do we use that to define our classifier?

## Information gain
Information gain is the entropy of the parent minus the weighted average of the entropy of the children that would result if you split that parent.
$$
InfoGain = S_{parent} - AVG(S_{children})
$$
The decision tree algorythm will try to maximize the information gain.
#### Calculating InfoGain
![[DT.example4.excalidraw.svg]]

<html >
<div style="background-color: palevioletred;  border-radius:10px">
<h3 style="margin:0; padding:7px 15px 0">Note</h3>
<p style="margin:0; padding:7px 15px">By default scikit uses 'gini index' as criterion to decide how to split the tree, as opposed to entropy. Either way works farily well, and in any case you can specify what criterion you want for your decision tree.</p>
</div>
</html>

## Strengths and weakneses

Easy to use and understand
They tend to overfit


