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