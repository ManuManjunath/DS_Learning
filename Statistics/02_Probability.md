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
