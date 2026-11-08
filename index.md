# Jenny Xu
jex004@ucsd.edu

D40 - Jun-Kun Wang

---

1. **What is the most interesting topic covered in your domain this quarter?**

    The most interesting topic covered in my domain this quarter is definitely sequential hypothesis testing and its application to algorithmic auditing. Unlike traditional statistical methods which are typically fixed, this approach allows for the continuous monitoring of a model's performance without a predetermined sample size. I found the mathematics behind the concept very intersting, like the Online Newton Step and dynamic wealth tracking.It completely changes how we think about evaluating machine learning models before and after deployment, treating model fairness as an ongoing requirement rather than a single checkpoint.

2. **Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

    One potential investigation I would like to pursue for my Quarter 2 Project is applying our sequential hypothesis testing algorithm to the financial sector, specifically focusing on corporate or sovereign credit ratings. Instead of evaluating demographic fairness in annual income, I want to use the framework to continuously monitor live market indicators, like bond yields or other indicators, to detect when a company or even country's financial stability has significantly shifted. The goal would be to build an early warning system that algorithmically signals when a credit rating should be reassessed in general and if we're feeling ambitious, whether it should be upgraded or downgraded. This investigation would also allow us to test how well the sequential algorithm handles economic data streams with high volatility and complicated distribution shifts.

3. **What is a potential change you’d make to the approach taken in your current Quarter 1 Project?** 

    If I could change our approach to the Quarter 1 project, I would implement an actual, live incoming data stream rather than attempting to simulate one by iterating through a static, already made dataset. While iterating through the Adult Census data was good enough for replicating the core mathematics of sequential hypothesis testing, it didn't really allow us to apply it properly to a scenario that may actually be happening in the real world. We also were able to control the "stream" of data to an extent in this quarter's project, but I would definitely instead want to try a project where there is asynchronous data ingestion and also latency. Setting up a true data pipeline would force us to handle real world deployment challenges, such as delayed API responses or missing demographic labels in the live stream too. Figuring out how to move from a local Jupyter environment to live production pipeline would make the auditing tool significantly more realistic.

4. **What other techniques would you be interested in using in your project?**

    I am highly interested in using Natural Language Processing (NLP) with interactive data visualization to monitor credit rating shifts. Rather than relying only on numerical market data, we could use LLM APIs or text embeddings to extract continuous "risk sentiment" features from streams of financial texts, such as earnings call transcripts or economics news. We would then take these textual classifications into our sequential hypothesis testing framework to detect when a credit rating upgrade or downgrade is needed. To make these algorithmic shifts easily interpretable, I want to build an interface to display a continuously updating graph with smooth animations that track the algorithm's results as new financial texts and numerical market data are processed. Combining live NLP feature extraction with dynamic visual storytelling would be a great way to translate hard to understand credit rating data and decisions into an easily understandable dashboard of some sort.