## Objective vs Subjective probability

Subjective Probability is based on personal feelings, experience, or judgement.  
Objective Probability is based on Statistics, experiments, mathematical measurements.  

2 Types of Objective Probability:  
- Classical Probability  
Number of desired outcomes / Total number of possible outcomes.  
Chance of getting heads when you flip a coin = 1 / 2 = 50%  
Chance of getting a "6" when rolling a dice = 1 / 6 = 16.7%

- Emperical Probability  
Based on experimental or historyc data.  
Number of times a specific event occurs / Total number of events.

## Principles of Probability

Probability of an outcome = No. of desired outcome / Total no. of possible outcomes  

#### Notations
P(A) = Probability of event A  
P(B) = Probability of event B  
P(A') = Probability of event not A  

#### Complement rule
If the probability of event A happening is P(A), the probability of event A not happening is P(A').  
If the probability of a team winning a game is 75%, the probability of the team not winning is 1 - 0.75 = 25%

#### Mutualy exclusive events
2 events are mutually exclusive if they cannot occur at the same time.  
> Additional rule for mutually exclusive events  
> $P(A or B) = P(A) + P(B)$  

Probability of getting 2 or 3 when you roll a dice =  
1/6 + 1/6 = 33.3%

#### Independent events
2 events are independent if the occurance of one event does not change the probability of the other.

> Multiplication rule for independent events  
> $P(A and B) = P(A) * P(B)$  

Probabiity of getting 2 consecutive heads during coin toss =  
1/2 * 1/2 = 25%

## Conditional Probability

Probability of anb event occurring, given that another event has already occurred.  

$P(A and B) = P(A) * P(B|A)$  
where P(B|A) = Probability of B, given A.

#### Baye's theorem

Prior Probability = Probability of an event before new data is collected.  
Posterior Probabiity = Probability of an event based on new data.  

$P(A|B) = (P(B|A) * P(A)) / P(B)$  
P(A|B) = Posterior Probability  
P(A) = Prior Probability  

For example:  
Overall chance of rain = 10%  
Days start off cloudy = 40%  
Rainy days start off cloudy = 75%

Event A = Rain
Event B = Cloudy morning  
Probability that it wil rain today, given that the morning is cloudy = (0.75 * 0.1) / 0.4 = 18.75%

## Discrete Probability

#### Random Variable
Represents the values for the possible outcomes of a random event.  
* Discrete Random Variable  
Has a countable number of possible values.(Countabe outcome)  
Eg: If you toss a coin 5 times, you can count the number of times you get Heads.
* Continuous Random Variable  
Takes all possible values in some range (Measurable outcome)  
For example, the height of a tree can be 5m or 5.2m or 5.21m or 5.215m

Sample space = Set of all possible values for a Random Variable.  
Sample space for a single coin toss = {Heads, Tails}  
Sample space for a single die roll = {1, 2, 3, 4, 5, 6}  

#### Binomial Distribution

For repeated trials, with each trial having 2 possible outcomes.  
Only 2 possible outcomes.  
Events are mutually exclusive.  
Each event is independent.

#### Poission Distribution

Calculates the probability that a certain number of events will occur during a specific time period.  
Number of events in the experiement can be counted.  
Mean no. of events that occur during a specific time period is known.  
Each event is independent.

## Continuous Probability

#### Normal Distribution (Gaussian Distribution)
Symmetrical on both sides of the mean and bell-shaped.  
Mean is located at the centre of the bell curve.  
Total area under the curve is 1.  

Emperical rule for normal distribution:  
68% of values fal within 1 Standard Deviation of the mean.  
95% of values fal within 2 Standard Deviation of the mean.  
99.7% of values fal within 3 Standard Deviation of the mean.  

#### Z-score
A measure of how many standard deviations below/above the population mean a data point is.  
Z-score = 0 if the value = mean.  
Z-score is positive if the value is greater than the mean.  
Z-score is negative if the value is less than the mean.  
$Z = (data point - mean) / standard deviation$  
