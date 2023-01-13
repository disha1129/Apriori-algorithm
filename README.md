# Apriori-algorithm
## Apriori algorithm was proposed by Agrawal and Srikant (1994).
Which means that customers who purchased diapers also purchased beer in the same basket.{diaper,beer} together is called itemset.
{diaper} is called the antecedent and the {beer} is called the consequent.
Both antecedents and consequents can have multiple items, e.g{diaper, milk} -> {beer,bread} is also a valid rule. Each rule is measured with a set of metrics.
### Metrics 
Such as Support, Confidence, and Lift are used to generate association rule.
#### -> Support:-
support indicates the frequencies of items appearing together in baskets with respect to all possible baskests being considered.
Support between X and Y, Support(X,Y) is given by
                support(X,Y)= N(XY)/N
Apriori algorithms uses minimum support criteria to reduce the number of possible itemset combinations, which in turn reduces computational requirements.
Hence, apriori algorithms computes support for each item independently and eliminates items with support less than minimum support.
#### -> Confidence 
Confidence measures the proportion of the transaction that contain X, which also contain Y. X is called antecedent and Y is called consequent.
                Confidence(X→Y) = Probability(X & Y) / Support(X)
                P(Y|X) = P(X & Y) / P(Y)
                where p(Y|X) is the conditional probability of Y given X.
#### -> Lift
Lift can be interpreted as the degree of assoication between two items. 
* Lift value 1 indicates that the items are independent(no association)
* Lift value less than 1 implies that the products are substitution
* Lift value greater 1 is a necessary condition of generating association rules.

