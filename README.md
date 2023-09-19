# Big-Data

## Introduction
Before going deep into the topic let's generally understand what is big data. Huge amount of data which you cannot be processed using the traditional methods is known as Big Data.
'Big Data' refers to an immense and continually expanding collection of data. This data is exceptionally large in size and has been growing at an exponential rate over time. Typically, we are familiar to working with data in sizes ranging from megabytes (such as Word documents and Excel files) to gigabytes (like movies and software code). However, when data reaches the scale of petabytes, equivalent to 10^15 bytes, it is categorized as Big Data.
Almost 90% of the data which we have today has been generated within the last three years.

### Examples of Big Data
Certainly, here are simpler explanations of the examples of Big Data:
1) A single jet engine can produce over 10 terabytes of data in just 30 minutes of flying. With thousands of flights happening daily, this adds up to many petabytes of data.
2) Every day, Facebook, Google, and LinkedIn collect more than 500 terabytes of new data from users and add it to their databases.
3) Weather stations and satellites gather massive amounts of data that's used to predict the weather.
4) Big telecom companies like T-Mobile and Verizon collect and analyze data from millions of users to create and offer better mobile plans based on user behavior.

### Types of Big Data
Generally Big Data is Classified into three types
1) Structured Data
2) Unstructured Data
3) Semi-structured Data

**Structured Data**:
Structured data is information that comes in a consistent, organized format, making it easy to store, find, and work with. 
One common example of structured data is the kind you find in a relational database management system.
For instance, think of a table in a database that holds information about employees. This table is a straightforward example of structured data.

**Unstructured Data**:
Unstructured data is information that doesn't follow a specific pattern or structure. A common example of unstructured data is when you have a mix of different types of data, like text files, images, and videos all jumbled together.
For instance, think about what you get when you do a 'Google Search.' The results you get from a Google Search are a prime example of unstructured data.

**Semi-structured Data**:
Semi-structured data is a type of information that combines both structured and unstructured elements.
An example of semi-structured data is 
1) Data stored in an XML file.
2) Comma Separated Values(CSV) File

## 6 ‘V’s of Big Data (or) Characteristics of Big Data ##

1. Volume
2. Variety
3. Velocity
4. Veracity
5. Value
6. Variability

   ![6 V's of Big Data](https://intellipaat.com/blog/wp-content/uploads/2020/02/Graphics-03.jpg)

                             

**Volume**:
The term "volume" refers to a large amount of data. The magnitude of data plays a critical role in determining its worth. When the
amount of data is extremely vast, it is referred to as 'Big Data'.
So, whether data is considered Big Data or not depends on how much of it there is. When handling Big Data, it's important to pay attention to its sheer size, or volume.

***Example:*** In 2016, worldwide mobile traffic was predicted to be 6.2 Exabytes (6.2 billion GB) per month. Furthermore, by 2020, we will have about 40000 ExaBytes of data.

**Variety**:
Variety is about the different kinds of data. When we talk about Big Data, it means we're gathering all sorts of data, like organized data, messy data, and partly organized data. This happens because we collect data from lots of different places, and these sources can be quite different from each other. So, variety in Big Data means dealing with a mix of data types from diverse sources.

Structured data is information that's been organized neatly, often with specific rules about how long it can be and what it should look like.

Semi-structured data is kind of like data that's partly organized but doesn't follow the usual rules. Think of it as data represented in a more flexible way, like log files.

Unstructured data is the opposite; it's messy data that doesn't fit nicely into the rows and columns of a typical database. It can be things like text, images, or videos that don't have a standard structure.

**Velocity**:
"Velocity" in Big Data means how quickly data is being collected. Data is pouring in rapidly from things like machines, networks, social media, and phones. It keeps coming in quickly and steadily. This affects how fast we can create and use data to meet our needs. To handle this speed, we might use data sampling, which is like taking a smaller portion of data to work with.

For example, Google gets over 3.5 billion search queries every day, and Facebook's user base is growing by about 22% each year.

**Veracity**:
When we talk about the veracity of big data, we're talking about how reliable and trustworthy the data is. Is it correct and of good quality? When dealing with big data that comes from different places, it's crucial to know where it came from, have details about it, and understand the circumstances when it was gathered. The better the data's veracity, the more valuable it is for making meaningful conclusions and helping an organization.

**Value**:
Value in the context of data means understanding why you're collecting or storing it. Is there a good reason or a specific goal it serves? If not, it might not be worth keeping. Also, when analyzing data, it's important to think about ethical concerns.

**Variability**:
Variability and variety are not the same. Imagine going to a coffee shop that offers six coffee flavors. If you order the same flavor every day, but it tastes different each time, that's variability. The same idea applies to data. If the meaning of the data keeps changing, it can make it really hard to make the data consistent and uniform.

## Phases of Big Data analysis

**Phase 1: Data Acquisition and Filtering**:
In the Data Acquisition and Filtering stage, we gather data from the sources we identified earlier. Then, we use automated filters to get rid of data that's either broken or not useful for our analysis.

The data can come in different forms, like a bunch of files you buy from a data provider or data you get through a service like Twitter. Often, especially when dealing with messy data from outside sources, a lot of the data we collect might not be helpful, so we throw it away during the filtering process.

**Phase 2: Data Extraction**:
Sometimes, the data we want to use for analysis isn't in a format that works with our Big Data system. This issue is more common with data from outside sources. 

So, we have a stage called Data Extraction, where we take this different data and change it into a format that our Big Data system can understand and use for analysis.

How much we need to change the data depends on what kind of analysis we're doing and what our Big Data system can do. For example, if we're working with text data, like web server logs or documents, and our Big Data system can already work with those, we might not need to change much.

![Data Extraction](https://blog.coupler.io/wp-content/uploads/2023/02/ETL-1024x483.png)

                   


**Phase 3: Data Validation and Cleansing**:
Incorrect data can mess up the results of our analysis. Unlike regular business data, which is usually well-organized and checked before use, the data we put into Big Data analysis can be messy and not checked for accuracy. It's often complicated, which makes it hard to set up rules to check its accuracy.

In the Data Validation and Cleansing stage, we create rules to check the data and remove any data we know is incorrect. For analysis done in batches, we can do this offline. But for real-time analysis, we need a more complex system that checks and cleans the data as it comes in from the source.

**Phase 4: Data Aggregation and Representation**:
Sometimes, data is in different places, and we need to put it all together by matching things like dates or IDs. Other times, the same data appears in different datasets, like birthdates.

In the Data Aggregation and Representation stage, we combine these different datasets to create a single, organized view of the data.

**Phase 5: Data Analysis**:
In the Data Analysis stage, we actually do the analysis work, which often includes different types of analysis methods. This stage might involve going back and forth several times, especially if we're trying to explore and discover patterns or connections in the data. Exploratory analysis, which we'll talk about later, is one way to do this, along with confirmatory analysis.

**Phase 5: Utilization of Analysis Results**:
After we share the analysis results with business users to help them make decisions, like through dashboards, there might be more ways to use these results. The Utilization of Analysis Results stage is about figuring out how and where we can use the data we've analyzed.

Depending on the problems we were trying to solve with the analysis, the results might help us create new "models" that give us fresh insights and a better understanding of patterns and connections in the data we looked at.

## Challenges in Big Data analysis 

**Data growth issues**:
One of the biggest problems with Big Data is storing these massive amounts of data correctly. The data stored in company data centers and databases is growing very fast. As time goes on, these datasets are getting bigger and harder to manage. A lot of this data is messy and doesn't fit neatly into databases because it comes from things like documents, videos, audio, and text files.

**Lack of proper understanding of Big Data**:
Companies often struggle with their Big Data projects because not everyone in the organization understands the ins and outs of data, like what it is, how to store and process it, why it's important, and where it comes from. 

For instance, if employees don't realize how crucial it is to store data properly, they might forget to back up important information or use databases incorrectly. This can lead to problems when we need to retrieve that important data later.

To tackle this issue, companies should organize workshops and training programs about Big Data for all their employees who work with data regularly. It's important for everyone in the organization to have at least a basic understanding of how data works.


**Confusion while Big Data tool selection**:
Companies can face challenges when trying to choose the right tools for Big Data analysis and storage. They might wonder whether HBase or Cassandra is better for storing data, or if Hadoop MapReduce is sufficient or if Spark would be a better choice for data analysis and storage. These questions can cause confusion, and sometimes companies make the wrong choices. This can lead to wasted money, time, effort, and work hours.


**Lack of data professionals**:
To use modern technologies and Big Data tools, companies require skilled experts like data scientists, data analysts, and data engineers. These professionals are experienced in using these tools to make sense of large datasets. However, many companies struggle to find enough of these experts because the tools have advanced quickly, but the professionals haven't kept up with the changes. To address this gap, steps need to be taken to train more professionals in Big Data skills.

**Securing data**:
One of the big challenges in Big Data is keeping all that data safe and secure. Sometimes, companies are so focused on figuring out, storing, and studying their data that they put off thinking about data security until later. But that's not a wise move because if data isn't protected, it can attract bad actors who can do harm. It's important to know that companies can face massive financial losses, up to $3.7 million, if their data is stolen or there's a security breach.

## References

[1] Thabet, Nasser & Soomro, Tariq. (2015). Big Data Challenges. Journal of Computer Engineering & Information Technology. 4. 10.4172/2324-9307.1000133.

[2] Rahman, Hamidur & Begum, Shahina & Ahmed, Mobyen. (2016). Ins and Outs of Big Data: A Review. 10.1007/978-3-319-51234-1_7.

[3] _Big Data Analytics Lifecycle | Big Data Adoption and Planning Considerations | InformIT. (n.d.)_. https://www.informit.com/articles/article.aspx?p=2473128&seqNum=11

[4] Khan, A., & Khan, A. (2023). Data Science vs Data Analytics vs Big Data. Intellipaat Blog. https://intellipaat.com/blog/data-science-vs-data-analytics-vs-big-data

[5]Yung, Z. (2023, February 23). Data extraction explained in Layman’s terms | Coupler.io blog. Coupler.io Blog. https://blog.coupler.io/data-extraction-guide/

 
