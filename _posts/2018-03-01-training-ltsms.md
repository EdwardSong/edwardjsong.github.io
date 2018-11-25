---
layout: default
title: My LSTM Network Notes - Training LTSMs
tags: [AI, ML, Artificial Intelligence, Machine Learning]
permalink: /machine-learning/long-short-term-memory-networks/training
category: Work
---

### Terminology

<ul>
    <li><strong>Backpropagation Training Algorithm</strong> - the mathematical method used to calculate derivatives and an application of the derivative chain rule and the training algorithm for updating network weights to minimize error.  The goal of the backpropagation training algorithm is to modify the weights of a neural network in order to minimize the error of the network outputs compared to some expected output in response to corresponding inputs.
        <ol>
            <li>Present a training input pattern and propagate it through the network to get an output.</li>
            <li>Compare the predicted outputs to the expected outputs and calculate the error.</li>
            <li>Calculate the derivatives of the error with respect to the network weights.</li>
            <li>Adjust the weights to minimize the error.</li>
            <li>Repeat.</li> 
       </ol>
    </li>
    <li><strong>Backpropagation Through Time</strong> - or BPTT, is the application of the Backpropagation training algorithm to Recurrent Neural Networks. In the simplest case, a recurrent neural network is shown one input each time step and predicts one output.
        <ol>
            <li>Present a sequence of time steps of input and output pairs to the network.</li>
            <li>Unroll the network then calculate and accumulate errors across each time step. 3. Roll-up the network and update weights.</li>
            <li>Repeat.</li>
        </ol>
    </li> 
</ul>

### Types
<ul>
  <li>No Notes</li>
</ul>

### Observations
<ul>
    <li>One of the main problems of BPTT is the high cost of a single parameter update, which makes it impossible to use a large number of iterations.</li>
    <li>One way to minimize the exploding and vanishing gradient issue is to limit how many time steps before an update to the weights is performed.</li>  
</ul>

### Further Reading

<ul>
    <li>http://ArXiv.org</li>
    <li>https://scholar.google.com/</li>
</ul>

[back](./)