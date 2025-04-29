# cs335---assignment-1-solved
**TO GET THIS SOLUTION VISIT:** [CS335 – Assignment 1 Solved](https://www.ankitcodinghub.com/product/cs335-assignment-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;111158&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS335 - Assignment 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Instructions

• This assignment should be completed individually.

• Do not look at solutions to this assignment or related ones on the Internet.

• The files related to the assignment are present in lab1-rollno.zip folder. Extract it and upload it on moodle in the same .zip format after completion and after replacing the string “rollno” with your actual roll number. For example, if you roll number is 00405036, then single zip folder that you will upload will be named “lab1-00405036.zip”. Also collate all the CS337 based theory solutions into ONE pdf file named answers.pdf. Include answers.pdf inside the zip folder mentioned above and submit the zip folder.

• Answers to all subjective questions need to be placed in single pdf answers.pdf including all plots and figures and uploaded.

• Only add/modify code between TODO and END TODO unless specified otherwise • In this assignment, you will perform Ridge, Ordinary Least Squares regression, and Bayesian Linear Regression.

• The code for all the questions should be written in provided ipython notebook only. Don’t modify the name/directory structure of the provided .zip file.

• Please make sure that your code runs in python 3.x. You shuld not import any new python libraries.

• Code should be written in the provided assignment 1.ipynb file only.

• All CS 335 questions will be auto graded with private testcases.

1 Ordinary Least Squares (OLS) Regression in one variable

1. Gradient descent is an optimization algorithm used to find the values of parameters (coefficients) of a function (f) that minimizes a cost function.

2. As for linear regression for the single variable case (that for 1 dimensional input x), we will use the standard y = wx + b slope equation where w is the line’s slope and b is the line’s y-intercept. To find the best line for our data, we need to find the best set of slope w and y-intercept in the form of b’s value.

3. To get started with, w and b are randomly initialized. However, for this assignment, we initialize them with zeros. Hence, we get a random line in the beginning. Our goal is to update these values so that the resulting line gives the least error.

4. We will use mean squared error ‘mse’ as the cost function, that calculates the error between the actual value output, and prediction from the hypothesis. mse =

5. This error function is typically convex – that is, cup-shaped. In simple terms, we can say that the result of convexity is that this error function typically has just one minimum (the global minimum).

6. When we start with random values of w and b, we get some value of y correspondingly. Error is minimum at the lowest point on this graph, so our goal is to move down the slope to finally reach the bottom-most point.

7. The slope of the tangent at any point on a graph is equal to the derivative of the graph w.r.t. input variables.

8. The slope of tangent at the bottom-most point on the graph is 0, i.e., the partial derivatives of mse at the bottom-most point are 0. To get to the bottom-most point, we have to move in the direction of the slope. That is, we will update values of w and b, such that we eventually get to the optimum values, where error function is minimum.

9. The update equations are

10. Here, ∇mse(wold,bold) denotes the ‘gradient’ vector ∇mse(w,b) evaluated at wold,bold. Further, ∇mse(w,b) is defined as

!

and η is called the ‘learning rate’ that determines how large the steps should be in the direction of the gradient. If the value of η is set to be very small, reaching the optimum value is guaranteed, but it will take a lot of time to converge. If η is very large, the values of w and b might overshoot the optimal values, and then the error will start to increase instead of decreasing. Hence, learning rate plays an important part in convex optimization.

Data Description

For this assignment, we assume a ground truth function y = f(x) = 1 − 3x − 2×2 + 2.5×3. However, as is typical of machine learning, we observe only noisy samples in the datasets that are provided. i.e. The dataset comprises of samples (x,y) such that y = f(x)+N(0,σ2) where σ is a hidden parameter that is not revealed to you. You have to use these samples to learn linear regression models using different algorithms.

1.1 CS337: Theory

1.2 CS335: Lab

2 OLS and Ridge Regression

2.1 CS337: Theory

Let N be the number of samples each having d features. Given the feature matrix X (N × d dimensional matrix) the outputs Y (vector of size N) and W the weights to be learnt, solve following

(b) For the minimum squared error loss function . Derive vectorized formula for (1 Mark)

2.2 CS335: Lab

Complete the following functions

(c) Complete the functions multivar reg grad and multivar reg closedform. Include the generated plots in your report. (1.5 + 1.5

Bayesian Linear Regression

Now, we will move to Bayesian Linear Regression. The fundamental difference here is that we model (w,b) as a Random Variable unlike the previous approaches that give point estimates of them.

For theory question, you will derive formulae for single variable regression. For programming part, we deal with multi-variable regression. We give you the formulae and you have to complete the code.

3 Bayesian Linear Regression

3.1 CS337: Theory

Let us consider the dataset where xi ∈ R and yi ∈ R. We need to learn the parameter w ∈ R. For convenience, let us assume the bias b = 0. (Note: For the programming part, you need to learn bias as well).

(b) Because we need a conjugate prior, we also assume that the data likelihood is Gaussian. i.e. p(y|x;w) = N(wx,1)

(e) From the expression above, we immediately realize that the denominator involves a daunting integral that is difficult to evaluate. Here is where we can leverage the conjugate prior assumption and find out p(w) analytically (ignoring the denominator).

(f) We can simplify the numerator of p(w|D) and thus deduce that

1) (Equation 1)

(g) We know that posterior is also Gaussian by virtue of conjugate prior. Thus posterior has the form ) (Equation 2)

3.2 MLE Estimate

(a) As we studied in class, in MLE estimate we maximize the (log) data likelihood i.e., w∗ = argmaxw p(D|w). For the above problem find the MLE estimate w∗ (1 mark)

(b) compare and comment on the MLE and Bayesian estimate (in the limit of ∞ data) that you obtain (0.5 mark)

3.3 CS335: Lab

(b) For this program, you will not encounter the problem mentioned in the question 2.1(d). Briefly explain why? (1 mark)

4 Conclusion

We saw multiple methods to learn the linear regression weights (w,b) for fitting the function f(x). Compare different methods and opine which one you think is superior. This is a open-ended question and we encourage you to compare for example running time, convergece, # iterations etc and explain briefly in your report with plots where applicable. (bonus 1 mark)
