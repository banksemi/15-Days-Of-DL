# Deep Learning
They wanted to solve the problem of human difficulties.

One of the methods is to try 'neuron'.
It consists of linear regression and activation functions.

![image](https://user-images.githubusercontent.com/17453822/68087059-751e1a00-fe95-11e9-991e-b6b1425983a6.png)


## Activation Function
A function that outputs y with proper handling of  input.

ex) Sigmoid function (y's range is 0 ~ 1)

ex) if f was sigmoid function,

f(X0 * W0 + X1 * W1 + ... + Xn * Wn + b) = f(z)
= 0~1

# XOR problem
Can the XOR problem be expressed as X0 * W1 + X1 * W2 + b?

Professor Minsky proves mathematically unsolvable
To solve this, It is needed a **multilayer neural net**.

** But couldn't gradient to each layer (~1970) **

*Can It solve XOR using multiple layers?*

(6 x X1) + (6 x X2) - 10 = Y1
(-5 x X1) + (-5 x X2) + 2 = Y2
(-10 * Y1) + (-10 x Y2) + 5 = Y

This may represent XOR.

### Solution

Backpropagation appeared by Paul Werbos, Dr. Hinton and others (Using ** Chain rule **)

# Backpropagation
Previously, the concept of gradient was used

It is also used for deep learning.


The biggest problem
How have solved a multiple layers gradient?
-> 
-> Can you get the derivative of Y as the input X passes through the layer? = dy/dx

Use **Chain rule** !

### Chain rule
<pre>
ex) Given formula
x * w0 + b0 = c
c * w1 + b1 = y


Things what we want : dy/dx
Things whay we can easily calculate: dy/dc, dc/dx
</pre>
**Chain rule**

<code>dy/dx = dy/dc * dc/dx</code>

** This means that even if the layers are complicated, they can be calculated linearly. **




# Reference
https://zamezzz.tistory.com/215
https://doorbw.tistory.com/140?category=706406
https://cyberx.tistory.com/128
