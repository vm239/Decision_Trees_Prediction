# Prediction
Prediction of student behavior has been a prominent area of research in learning analytics and a major concern for higher education institutions and ed tech companies alike. It is the bedrock of [methodology within the world of cognitive tutors](https://solaresearch.org/hla-17/hla17-chapter5/) and these methods have been exported to other areas within the education technology landscape. The ability to predict what a student is likely to do in the future so that interventions can be tailored to them has seen major growth and investment, [though implementation is non-trivial and expensive](https://www.newamerica.org/education-policy/policy-papers/promise-and-peril-predictive-analytics-higher-education/). Although some institutions, such as [Purdue University](https://www.itap.purdue.edu/learning/tools/forecast.html), have seen success we are yet to see widespread adoption of these approaches as they tend to be highly institution specific and require very concrete outcomes to be useful. 

I have built three prediction models within the classification tree type, in order to predict if students enrolled into particular courses in the semester complete the course or not. This enables us to understand how better to allocate valuable resources while allowing students to have the freedom to choose and sample courses.

The data used in this project comes from a university's registrar and is first run through a scatterplot matrix in order to do an initial visualization of the available information.

### Scatterplot Matrix

<img width="791" alt="Scatterplot matrix" src="https://user-images.githubusercontent.com/70535288/122102276-e45e3d00-ce32-11eb-8c03-71c719ef1746.png">

We notice that for the categorical variables, we are unable to gather meaningful visualization with a scatterplot, hence we use a jitter. Note that complete, our desired variable of interest which denotes if a student completes a course or not, is a categorical variable.

<img width="714" alt="CompleteVsYear" src="https://user-images.githubusercontent.com/70535288/122102592-3737f480-ce33-11eb-8cf7-d13fb7d1548b.png">

<img width="685" alt="CompleteVsEntrancescores" src="https://user-images.githubusercontent.com/70535288/122102629-40c15c80-ce33-11eb-9448-d7dff6d66ffa.png">

<img width="699" alt="CompleteVsCourses" src="https://user-images.githubusercontent.com/70535288/122102663-4ae35b00-ce33-11eb-8e7b-18b2d91a66af.png">

<img width="689" alt="CompleteVsCourseID" src="https://user-images.githubusercontent.com/70535288/122102691-533b9600-ce33-11eb-9360-ad0ffa5e7df6.png">

We then clean and prepare our data for the three models, and generate summaries for each based on the parameter of Accuracy of the model.

___

## The CART Tree
<img width="729" alt="Cart tree model" src="https://user-images.githubusercontent.com/70535288/122102842-83833480-ce33-11eb-8c1d-1d20b84a912f.png">

### The CART Tree summary
<img width="576" alt="Cart Tree summary" src="https://user-images.githubusercontent.com/70535288/122102847-854cf800-ce33-11eb-8b87-2573ef16b7a9.png">

___

## The Conditional Inference Tree Model
<img width="711" alt="Conditional inference model" src="https://user-images.githubusercontent.com/70535288/122102849-867e2500-ce33-11eb-8365-f77115d7e666.png">

### The Conditional Inference Tree summary
<img width="394" alt="Conditional inference summary" src="https://user-images.githubusercontent.com/70535288/122102856-87af5200-ce33-11eb-8737-21ac92599689.png">

___

## The C5.0 Tree Model
<img width="681" alt="C5 0 Model and summary" src="https://user-images.githubusercontent.com/70535288/122102828-7ebe8080-ce33-11eb-8a3a-d84046154867.png">

### The C5.0 Tree summary
<img width="396" alt="C5 0 summary" src="https://user-images.githubusercontent.com/70535288/122102836-81b97100-ce33-11eb-819d-e1d797ae95c4.png">

___

A comparison of the different models are seen in this graph, as well as in the RMD and HTML files in this repository.

<img width="730" alt="Three models comparison graph" src="https://user-images.githubusercontent.com/70535288/122102864-89791580-ce33-11eb-88eb-c4a563d373bb.png">

These models provide different accuracy rates and the best out of them is seen to be the Conditional Inference Model. This model could be used for the most accurate predictions of students who are likely to complete courses they have enrolled into, and could solve the problem of optimum allocation of resources.

___

## Future Work
- Predictions provide a wide array of benefits and can be utilized across different industrial and service sectors.
- Accuracy of different models of prediction can be sharpened by selecting variables of interest from a large dataset, and then running them through different packages for more customised results.
- The type of variables within the available data expand the horizons on the different prediction models which are possible and suitable, based on which further investigation can be carried out beyond Classification Tree models.

___

## Tools
- R and R Studio
- R packages
- Git
- GitHub

___

## Author
Vidya Madhavan, MS candidate for Learning Analytics, Teachers College, Columbia University

---

