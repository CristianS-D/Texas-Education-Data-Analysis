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


### Clustering Texas School Districts; A Work in Progress
I've worked with education data for about a year and a half, and something I've felt intuitively the whole time is that there are better ways to benchmark school districts than what's currently used. This project is my attempt to find out if I'm right.
The Question

If you group school districts by operational and demographic factors; teacher pay, teacher experience, student-teacher ratio, per-pupil spending, and others I'm still working through; do meaningful clusters emerge? And if they do, what can we learn from them?
The benchmarking angle was the original motivation, but the more I work on this, the more I think the real value might be elsewhere: identifying which districts do a lot with a little, understanding what separates high-performers from low-performers within a cluster, and finding the levers that could actually lift the lowest-performing schools.

A specific example I keep coming back to: Dallas ISD and a small rural district might spend the same amount per student, but Dallas likely benefits from economies of scale that produce better outcomes. Where's the threshold? What would it take to replicate that?
The Data

STAAR performance data for Texas school districts, 2013–2025, downloaded from public sources, cleaned, merged, and feature-engineered over several months. This project has been as much about learning pandas and data science in practice as it has been about answering the question.
What I've Tried and Learned

This has been a learning project as much as a research one. Some of the concepts I worked through along the way:

Beta-binomial smoothing; for stabilizing teacher counts in small districts
Z-scores and bimodal distributions; exploring the shape of teacher experience variance
Euclidean distance; the formal name for something I'd been reasoning through intuitively for years
HHI (Herfindahl-Hirschman Index); used to determine ethnic homogeneity
Data imputation; handling the gaps that come with real, messy public data

A few approaches I explored turned out to be dead ends for this particular problem; which is fine. That's part of it.
Where It Stands

Honest status: I haven't found meaningful clusters yet with the current feature set. The groupings I've tried so far don't tell a clear story.
My next step is pulling in new data sources, engineering better features, and running the clustering again with a more informed setup. I've got about a month left of energy I want to put into this before I either find something worth sharing or open it up for others to continue.
31 commits since February 7th. Some weeks nothing, some weeks every night after work. It's a side project; and because of that there is no deadline tha takes away the ability for play; which is one of the best tools for novel discovery. 
If You Want to Pick This Up
If I don't find something meaningful in the next round, I'll publish the full cleaned dataset, feature engineering pipeline, and everything I've tried so far. If this question interests you, reach out.

Work in progress. Last updated April 2025.