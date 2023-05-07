Download Link: https://assignmentchef.com/product/solved-int301-lab-4-further-practice-with-perceptrons
<br>
Further Practice with Perceptrons

Demo:

Analyze the given program PerceptronExample, which consists of following parts:

<ol>

 <li>(1)  Prepare mydata by generating 2 dimensional linearly separable data.<pre>        mydata = rand(500,2);</pre><pre>        % Separate the data into two classes</pre><pre>        acceptindex = abs(mydata(:,1)-mydata(:,2))&gt;0.012;        mydata = mydata(acceptindex,:); % data        myclasses = mydata(:,1)&gt;mydata(:,2); % labels</pre><pre>       [m n]=size(mydata);</pre>You may check the data distribution using:<pre>          scatter(mydata(:,1),mydata(:,2))</pre></li>

 <li>(2)  Train the perceptron by calling the function PerceptronTrn with the prepared training data (x, y), which will return the connection weights, the bias, and the number of iteration;</li>

 <li>(3)  Test the trained Perceptron model with the testing data (xt, yt), by calling another function PerceptronTst, which will return the testing error;</li>

 <li>(4)  Display the two classes of data points with a separating line.</li>

</ol>

Exercise:

<ol>

 <li>(1)  The Perceptron training function uses a learning rate 0.5 and a threshold 0.5. Change these two parameters, e.g. learning rate 0.1 and threshold 0, and observe the differences;</li>

 <li>(2)  Revise the program to calculate the Root-Mean-Square (RMS) error for every input data points and display the error curve, i.e. RMS vs. iteration.</li>

</ol>