# State of Learning During Covid: EdTech Product Data Across US School Districts

## Objectives:  
* Comment on student's learning during the pandemic by:
    * Analyzing _engagement index_ (_total page-load events per one thousand students of a given product and on a given day_) across 372 EdTech products over a period of 1 year starting from January 2020 (pre-covid) to January 2021 
    * Exploring variations in engagement indices across school districts and investigating why they look different
    * Commenting on the generalizability of findings, i.e. whether this analysis be extrapolated to make claims about certain states, the country as a whole etc.

## Key Takeaways:
1. We can segment products and school districts based on _mean engagement index_ across time, **which is used as a proxy metric for learning**. However, we cannot generalize our observations over states or the country. Our analysis is not generalizable because we only have a small sample of school district data across states. We cannot comment on the representativeness of our sample because district anonymity has been preserved in the dataset. 

### Product breakdown:

2. Our 372 EdTech products are divided into 3 broad categories by function: LC (Learning and Curriculum), which dominates with almost 70% of products in that category, CM (Classroom Management),and SDO (School & District Operations), which have an almost equal split. Further, we split products into 4 categories by _mean engagement index_:  
    * l1 products have a _mean engagement_ index between 10-100; i.e. on average, a product in this category had at most 100 page load events per 1000 students on a day, or 0.1 page load event per student per day. This indicates low engagement over time
    * l2 products have a _mean engagement_ index between 100-1000
    * l3 products have a _mean engagement_ index between 1000-10000
    * l4 products (only 1) _mean engagement_ index of ~11K. While we could have added this to the previous bucket or removed it as an outlier, it was interesting to independently look at the usage of this product across time and across school districts

3. Within the ~270 LC (Learning and Curriculum) products:
    * the majority (63%) fall in l1 catgeory, which means, on average, they had a _mean engagement index_ between 10-100
    * 35% fall in l2 category, which means they were utilized more, but still at a _mean engagement index_ of <1000 per day, on average, they had less than 1 session per student per day
    * Only 4 products fall in l3 and l4 categories - these products were likely used more frequently. It would be interesting to investigate whether this was self-driven usage or through school policies

4. Within the ~63 CM (Classroom Management) and SDO (School & District Operations) products:
    * 5 are l3, and 14 are l2. Engagement of these products would have likely gone up during Covid. We could examine the time series usage of the 5 l3 products and compare with the 14 l2 - did the l3 ones see a spike post-Covid, and where that potentially happened

5. When we examine _mean engagement index_ of l1, l2, l3, l4 products over months, we notice the same pattern: **mean engagement increases from January till March, then drops till July and then picks up again**. The troughs likely coincide with school closures due to summer vacation or other national holidays. l1 and l2 pre and post covid monthly means seem similar, which indicates that these products were utilized more or less the same way before and after the pandemic. However, this is not the case for l3 and l4 products, l4 being just one - Google Docs. L3 products also witness higher mean engagement post Covid, which indicates these products were adopted more frequently, either by the same schools or by new schools. There are 8 l3 products, out of which 4 are Google owned (Classroom, Youtube, Meet and Forms). 

6. When we examine the same metric for weekdays, it seems clear that l1 products have the same means pre and post covid, which means their usage was low but was self-driven. l2 products have a clear spike in daily means, and have large values even in March, right around the onset of Covid. This means their usage was more likely driven by schools, just like for l3 and l4 products. 

### District breakdown:
_git upload pending_


### Interactive Visualizations:
_git upload pending_


### About the Dataset:
For We have data from the following 3 buckets:
The engagement data are based on [LearnPlatform](https://learnplatform.com/)’s Student Chrome Extension. The extension collects page load events of over 10K education technology products, including websites, apps, web apps, software programs, extensions, ebooks, hardwares, and services used in educational institutions. The engagement data have been aggregated at school district level, and each file represents data from one school district. The product file includes information about the characteristics of the top 372 products with most users in 2020. The district file includes information about the characteristics of school districts, including data from [National Center for Education Statistics (NCES)](https://nces.ed.gov/), [The Federal Communications Commission (FCC)](https://www.fcc.gov/), and [Edunomics Lab](https://edunomicslab.org/).