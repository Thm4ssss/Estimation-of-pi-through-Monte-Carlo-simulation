## Estimating the value of $\pi$ by performing a Monte-Carlo Simulation

The goal of this project is to estimate the value of $\pi$ by using a Monte-Carlo simulation. <br>
To do so, we consider a square of side $2R$, and we draw a circle of radius $R$ on its center. Thus, the area of the square is: $4R^2$. The area of the circle is $\pi R^2$.<br>

Now, let's consider a point in the square. The probability for the point to be also in the circle is equal to :
$$ P=\frac{\pi R^2}{4R^2}=\frac{\pi}{4} $$

We'll estimate this probability with a Monte Carlo simulation.<br>

The logic is simple : we generate $N$ points in the square, with a uniform probability for each component. Thus, we compute the number of points that are in the circle, dividing this number by the number of points gives us the estimate probability of being in the circle.<br>

It is possible in the code to change the number of simulations to see how the accuracy and the time to compute change.<br>