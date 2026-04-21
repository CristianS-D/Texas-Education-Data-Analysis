# District Categorization on Various Demographic Indicators
#### Multidimensional Peer Grouping for School District Benchmarking
1. Objective

The goal of this project is to develop a more accurate bench marking system for school district performance. Current methods often rely on state averages or geographic neighbors as points of comparison. However, these benchmarks are often flawed because they ignore vast disparities in socioeconomic status and district community makeup.

2. Hypothesis

I hypothesize that school district outcomes are more accurately predicted and compared by grouping districts based on socioeconomic and both ethnic and non-ethnic demographic data rather than location. Specifically, relationships I anticipate seeing:

    Teacher Compensation, Teacher Experience Levels, and Student-Staff Ethnic Homogeneity will be primary drivers of performance variance.

3. Methodology: Clustering algorithm

To define these "statistical peers," I intend to utilize a K-Nearest Neighbors (KNN) or similar clustering algorithm. By plotting districts in a multi-dimensional space, we can identify the "nearest" districts based on:

    Economic Disadvantage Percentage: The ratio of students qualifying for free/reduced lunch. 

    Ethnic Homogeneity Index: The alignment between student demographics and staff demographics.

    Teacher Salary Scales: Adjusted for regional cost of living.

    Funding per Student: Total operational expenditures.

4. Considerations

    Some considerations I'm intentionally overlooking due to complexity keeping this project easy for now are...

    School districts who receive CEP funding are not incentivized to accurately report "Eco Dis" (Economically Disadvantaged) status due to the fact that they already receive the free/reduced lunch funding.

    Additionally, when looking at teacher compensation, not being able to compare to the geographic cost of living in an area will limit my ability to most accurately cluster those school districts. A teacher who gets paid $40,000 in Dallas versus $40,000 in a rural town might be experiencing different costs of living.

    

5. Business Use Case

    Districts often receive funding via grants and sub-grants, where they are expected to hit certain performance metrics. When benchmarked, they are compared to neighboring school districts or other districts within the same sub-grant to see how they are performing.

    A common issue is that school districts appear to be underperforming relative to their neighbors, but I suspect the underlying drivers of these performance issues aren't necessarily due to a lack of effort by the district. Instead, they are due to differences in district makeup—whether it be demographic data, compensation, teacher experience, etc.

    To more accurately tell how the schools are performing and compare them on the same playing field, we can better assess if a school district is growing realtive to it true peers. 


### On Clustering School Districts, Frustration, and Why I'm Still Doing This

I have worked with education data for going on nearly a year and a half now, and something I felt very intuitively based on what I've seen is that there are better ways to cluster these school districts.

I started out by downloading STAAR data for school districts in Texas from 2013 to 2025, and cleaned those up, merged them, spent a lot of time cleaning and doing a lot of feature engineering; mostly to learn pandas and data science along the way; spending sometimes weeks on learning statistics and Bayesian statistics, statistical methods that I learned after a couple days were obsolete. But again, it being a side project, I'm very okay with that because I have no deadline.
This is something I work on. I work with student data in a full-time job, but this question and my method of how I wanted to get there were not something I felt I'd be able to successfully pitch to an organization, and have the right amount of time allocation for. Mostly because I'm relatively new to pandas in any competent sense. And I wanted the ability to express myself and my interests very freely in my studies and journey. I think a lot of pressure that corporations put on people takes away the ability for an artist or a scientist or any competent individual to dance or play. They're required to work within a rigid framework that doesn't really allow a whole lot of innovation or growth.

After going on three months of work on this; I started on February 7th and it's April 20th now; I've only had 31 commits. Some weeks I don't work on it, some weeks I work every day after work from when I get home to when I go to bed. It really just depends on my availability and interest level because I have other hobbies and interests, yet this one has taken a significant amount of time. Mostly because I really care about the question. I believe there's a lot to learn from it, both in my professional skill set but also in the question it's answering.

Which is: are there better ways to benchmark school districts? From that I think there's more than just benchmarking; what I'm noticing now is benchmarking might not even be the best outcome of this. But are there ways to identify; the questions that come from this as I've been working on it are; if you group school districts based on certain operational and demographic factors, such as how much do they pay teachers, what's their teacher experience, what's the student-teacher ratio, what's the pay per pupil, etc., and I don't know what other features because I'm still working on it as I haven't found any statistically significant groupings or any valuable groupings.
The highlights of my growth: I've learned the beta-binomial smoothing, z-scores, bimodal distributions, the HHI index if I want to get really granular. I've learned Euclidean distance, which is a concept I've actually already understood for years; I didn't know the formal name. It's not even something I applied computationally, but just in my head. I work three-dimensionally and Euclidean distance is the way I view things in three-dimensional space normally. So it's really cool to put a word to it. Data imputation is another thing I've learned.

Some of the things I'd like to know: why are certain districts in the groups that I theorize have to exist; and I haven't found them yet. Are any of the groups performing better? Why are they performing better, and how can we apply those lessons to other school districts? Do some schools do exceptionally well with less money? If you look at a school district like Dallas, perhaps they spend the same amount of money per student as a school district in a rural part of Texas, but maybe there are economies of scale and they produce better outcomes because they have more resources and more scale. And what is the threshold that we could use to lift the lowest schools up?

Also, using these cluster methods to see if different benchmarks better represent things.
As of now I have to take a pause, as my frustration has gone very high and I do not see useful outcomes with the current features I've selected. I will probably be downloading new data sets, cleaning them, and applying those new features I create to the clusterings. I might apply one more month of work to this. But if I don't see anything, I will put the project out and ask if anybody else wants to pick it up. Until then, I think I have one more month.