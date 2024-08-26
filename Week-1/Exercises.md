## Bonferonni's Principle

- **1.2.1**

(a) The number of days of observation was raised to **2000**.  
Original sentence: *We shall examine the hotel records for 1000 days.*

(b) The number of people observed was raised to **2 billion** (and there were  
therefore **200,000** hotels).  
Original sentence: *Hence, there are 100,000 hotels*

(c) We only reported a pair as suspect if they were at the same hotel at the  
same time on **three different days.**
Original sentence: *An “event”  in this sense is a pair of people and a pair of days, such that the two people were at the same hotel on each of the two days.*

Number of suspected pairs?

Chance that they will visit the same hotel three days = $10^{-9}\cdot 10^{-9} \cdot 10^{-9}$ = $10^{-27}$

Number of pairs of people = $\binom{2\cdot10^9}{2}$ = 1999999999 * $10^6$ or around $n^2/2$ = $2\cdot10^{18}$
> Confirm with math.comb

Number of "three days" = $\binom{2000}{3}$ = 1331334 * $10^3$  

The expected number of events that look like evil-doing is the product of the **number of pairs of people**, **the number of pairs of days**, and the probability that any one pair of people and pair of days  is an instance of the behavior we are looking for.

Expected number of events (with approximation) = Number of pairs of people × Number of "three days" × Probability = $2\cdot10^{18}$ x 1331334 $\cdot$ $10^3$  x $10^{-27}$
$\approx 2.66??$

- **1.2.2**

Assumption: same set of 10 items at some time during the year

$10^6$ people
100 times a year,  10/1000 items

Ways to buy 10 unique items = $\binom{1000}{10}$
Probability person B buys the same as person A = $\frac{1}{\binom{1000}{10}}$
Pairs of $10^6$ people = $\frac{10^{12}}{2}$  = $5\cdot 10^{11}$ by  $n^2 / 2$ approximation

Expected number=Number of pairs of people × Number of visits× Probability of a match = ... 100 $\cdot$ ...

< 1
## Document Frequency

- **1.3.1**
(a)
$$
\text{IDF} = \log_2\left(\frac{10\,\text{million}}{40}\right) = \log_2(250\,\text{thousand}) \approx 17.9 \approx 18
$$

(b)
$$
\text{IDF} = \log_2\left(\frac{10\,\text{million}}{10\,\text{thousand}}\right) = \log_2(1\,\text{thousand}) \approx 9.97 \approx 10
$$

- **1.3.2**

Given:
- **Number of documents** ($N$) = 10 million
- **Word $w$** appears in 320 documents
- **Maximum frequency in a document** ($\text{maxfi}$) = 15

(a) When $f_{ij} = 1$:

$$
\text{TF} = \frac{1}{15}
$$
$$
\text{IDF} = \log_2\left(\frac{10\,\text{million}}{320}\right) \approx 14.92
$$
$$
\text{TF} \times \text{IDF} \approx \frac{1}{15} \times 14.92 \approx 0.9947
$$

(b) When $f_{ij} = 5$:

$$
\text{TF} = \frac{5}{15} = \frac{1}{3}
$$
$$
\text{IDF} = \log_2\left(\frac{10\,\text{million}}{320}\right) \approx 14.92 \quad (\text{same as above})
$$
$$
\text{TF} \times \text{IDF} \approx \frac{1}{3} \times 14.92 \approx 4.97
$$

- **1.3.3**

Explain with buckets (0 to 14)
relatively prime c
must *gcd(c, 15) = 1*
e.g. 1, 2, 4, 7, 8 ...


