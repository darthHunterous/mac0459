# [03 - Concrete Introduction to Python Probability](http://nbviewer.jupyter.org/url/norvig.com/ipython/Probability.ipynb)

* **Laplace Probability Definition**
    * Fraction whose numerator is the number of favorable cases and whose denominator is the number of all possible cases
* **Probability Vocabulary**
    * **Experiment**
        * Ocurrence with a certain observable outcome
    * **Outcome**
        * Result of a experiment
    * **Sample Space**
        * Set of all possible outcomes
    * **Event**
        * Subset of possible outcomes with the interested property
    * **Probability**
        * Number of favorable outcomes from the ssample space divided by the total number of cases in the sample space (assuming all outcomes equally likely)
<br><br>
* **Output Python Integer Fractions**
    * <code>from fractions import Fraction</code>
* **Numerator as Intersection of Event and Space**
    * <code>len(event & space)</code>
    * We only want to consider events which are included in the sample space
* **Combinations in Python**
    *  <code>import itertools</code>
    * <code>itertools.combinations(items, n)</code>
* **Factorial in Python**
    * <code>from math import factorial</code>
<br><br>
* **Frequency**
    * How often an outcome occurs
    * Can be a count or a ratio
* **Distribution**
    * Mapping from outcome to frequency for each outcome possible in the sample space
* **Probability Distribution**
    * Normalized distribution so the sum of frequencies is 1
<br><br>
* **Newton and Pepys Dice Problem**
    * [Stephen M. Stigler - Isaac Newton As A Probabilist](http://fermatslibrary.com/s/isaac-newton-as-a-probabilist)
    * Which is more probable?
        * Six dice tossed independently with at least one "6"
        * Twelve dice tossed independently with at least two "6"
        * Eighteen dice tossed independently with at least three "6"
    * Solved with a random variable X ~ Binomial (N, p)
        * X denotes the number of "6s"
        * N is the number of dice
        * p is the probability of getting a "6"
    * Results
        * P (X >= 1) = 31031 / 46656 = 0.665
            * For N = 6 and p = 1 / 6
        * P (X >= 2) = 1346704211 / 2176782336 = 0.619
            * For N = 12 and p = 1 / 6
        * P (X >= 3) = 60666401980916 / 101559956668416 = 0.597
            * For N = 18 and p = 1 / 6
<br><br>
* **Central Limit Theorem**
    * For a sum of a collection of random variables, the larger the collection, the closer the sum will be to a *normal distribution*
<br><br>
* **Cutoff Game**
    * **A, B**
        * Cutoffs chosen by player A and player B
        * Lower bound of the range to be accepted by a player
    * **a, b**
        * Actual random number received
    * What cutoff **A** maximizes chance of winning, which means, maximize P(a > b)?
        * Performing the statical analysis gives that the optimal cutoff is around 0.61803
        * Close to the Golden Ratio