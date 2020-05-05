# ImSafe Science

Every day, several reports about COVID disease trajectory and prevalence are published. The volume of findings, along with the complexity of sampling strategies, presents a challenge to researchers and policy makers alike for making clean inference based on data.

For instance, it

1. an individual's health state (e.g. **infected**, **symptomatic**, etc.), 
2. actions (e.g. **hospitalization**, **getting tested**, etc.), and
3. and factors suspected of affecting either of the above (e.g. **access to testing**, **test type**, etc.)

We will use this ontology to organize scientific findings that estimate either  
1) the probability of being in a given state (e.g. being positive given a serology test result), or
2) the probability of transitioning from one state to another (e.g. probability of death given symptoms and patient characteristics)

We show that this map provides a useful framework for summarizing findings while making their assumptions more explicit.

We believe that this framework can help in making optimal inferences from existing research and prioritizing hypotheses for future research.

## Terminology
`exposure`
: coming into contact with the virus through air or surfaces.

`infection`
: the virus has begun reproduction within the body, 


## Disease states



p(disease)<sub>x, t</sub>
: Probability of individual to have the disease at time *t* and location *x*. Agnostic of patient characteristics, this is simply the average `prevalence` of the disease at time *t* and location *x*.
: sources: 
   1. [Estimating the Prevalence of COVID-19 in the United States: Three Complementary Approaches](https://www.medrxiv.org/content/10.1101/2020.04.18.20070821v1)

p(symptoms | disease)
: Probability of developing symptoms given a disease

p(receiving test | symptoms, access)
: in the US, this probability has largely been conditioned on symptom on-set -- i.e. asymptomatic carriers have been undetected. We feel that . In other locations, where 

p(test_positive | disease, test_sensitivity, time_of_test)
: probability that a test returns positive, given that the individual has the disease, and the test's false positive rate.

p(test_negative | disease, test_sensitivity, time_of_test)
: probability that a test returns negative, given that the individual has the disease, and the test's false positive rate.

p(immunity | test_positive, time_of_test)
: 
