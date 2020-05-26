## Workbook - Aaron Kane

_ACME Corporation is looking for devs with an understanding of Rails. The following set of questions relate to this RfQ-requirement._

# Q1 - Describe the architecture of a typical Rails application

Rails architecture follows the Model-View-Controller(MVC) design pattern where the major components of the application are organised into three layers in order to achieve a "separation of concerns". This separation of concerns increases the application's robustness and testability as each component has no knowledge of the other.

## The Model
The model is the application's data structure and has no knowledge of the user interface. It handles the data logic for the rails application. The model layer communicates with the database and makes it available through the controller. The model is typically located in the app/model folder.

## The Controller
The controller layer is the mediator between the model and the view and controls the flow of the application. In a typical rails application the controller will query the database and organise it in order to pass it to the view.

## The View
The view represents the data to the user. In a rails application this is typically done with embedded ruby or haml. Rails views are typically located in the app/views folders.


## Diagram of a typical rails application
![](docs/rails_mvc.png)
[link to image source](https://i.pinimg.com/originals/6e/f1/8d/6ef18dd3444ddb80c86ffb169bbd6e98.png)

### **Description of the above digram** - 

The browser will send a request to a web server. The web server that is hosting the application will then connect to the routing of the application. The routing engine then communicates with the controller. The controller then communicates with the model in order to pass the data to the view. The view then displays the data and sends it to the web server which then displays it to the browser.

# Q2 - Identify a database management system (DBMS) commonly used in web applications (including Rails) and discuss the pros and cons of this database
Postgresql or simply postgres is a general purpose database management system used worldwide. It was initially release in 1996 and is an open source database system and is used by many different applications. With its' popularity PostgreSQL has gained a large open source support but even with this support there are still some limitations.

## Exploring the PROS - 
- PostgreSQL is scalable and integrates well with multiple applications.
- Open source making it free to use in any applications as well as the ability for developers to work on and improve it.
- PostgreSQL supports JSON
- Has many built in functions to assist with development
- Number of GUI to manage the database such as PGAdmin4
- Support NoSQL

## Exploring the CONS - 
- PostgreSQL being open source can also have downsides. There is no official support and improvements and updates rely on the community. This means if community support diminishes developers will pivot away from using it.
- Speed can be an issue when performing large tasks.
- Slower than other DBMS such as MySQL
- Documentation lacks when compared to other popular DBMS

REFERENCES

https://www.quora.com/Is-PostgreSQL-a-distributed-and-scalable-database

https://www.keycdn.com/blog/popular-databases

https://www.quora.com/What-are-the-advantages-and-disadvantages-of-PostgreSQL

_ACME Corporation is very big on project management, documentation and process. This will be a key metric in their decision to award the project. The following set of questions relate to this RfQ-requirement._

# Q3 - Discuss the implementation of Agile project management methodology
Agile project management is methodology for delivering projects based on iteration. Agile can also be considered a mindset that can respond to ever changing requirements of the project. Agile has become a popular mothodology worldwide for project management as there are numerous advantages to this approach. Firstly, agile is implemented using the scrum flow where teams deliver products in short cycles as opposed to one delivery at the end of a project. Agile is focused on user feedback. User feedback is essential in agile development as iterations are made to the product based on such feedback. The feedback is documented and placed in the backlog. Another advantage to using the agile approach is user stories. User stories give developers insight into client needs by putting the end user at the centre of feature development. User stories typically contain a brief description of the needs of the user for example - "as a user I should be able to register an account". After completing these features feedback from end client is tested to guage customer satisfaction. Agile can also be seen as a mindset where teams must have a flexible mindset in order to respond accordingly to changing demands of a project.

REFERENCES

https://www.visual-paradigm.com/guide/agile-software-development/what-is-user-story/

https://www.guru99.com/waterfall-vs-agile.html



# Q4 - Provide an overview and description of a standard source control workflow

Some popular Git workflows include basic, gitflow, feature branch workflow and integration-manager.

Here the feature branch workflow will be discussed - 

When implementing the feature branch workflow there should be one main branch typically called master with other branches pulling from it. It starts with all developers pulling from the master branch and creating a feature branch. This way changes will be committed to the feature branch while the master branch remains unaltered. When the developer has finished the feature a pull request is made. A pull request is an opportunity for the development team to discuss features in greater detail and once reviewed the feature branch can merge with the master branch. In most cases different features will be worked on simultaneously this can cause merge conflicts. To avoid merge conflicts, before submitting a pull request the developer must first pull from the master branch to have the lastest version of the project.

![Feature-branch workflow](docs/feature-branch.png)
[Link to image](https://buddy.works/blog/images/feature-branch.png)

REFERENCES
https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow

https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows



# Q5 - Provide an overview and description of a standard software testing process (e.g. manual testing)

_Having suffered several cyber attacks in the past and resultant remedial audits ACME Corporation takes compliance, security and privacy very seriously. The following set of questions relate to this RfQ-requirement._

# Q6 - 	Discuss and analyse requirements related to information system security and how they relate to the project

# Q7 - Discuss common methods of protecting information and data and how you would apply them to the project

# Q8 - Research what your legal obligations are in relation to handling user data and how they can be met for the project

_ACME Corporation has specifically requested the app to be based on a relational database. The next set of questions relate to this RfQ-requirement._

# Q9 - Describe the structural aspects of the relational database model. Your description should include information about the structure in which data is stored and how relations are represented in that structure.

# Q10 - Describe the integrity aspects of the relational database model. Your description should include information about the types of data integrity and how they can be enforced in a relational database.

# Q11 - Describe the manipulative aspects of the relational database model. Your description should include information about the ways in which data is manipulated (added, removed, changed, and retrieved) in a relational database.

_The efficiency of an app (i.e. site) and the algorithms used are of the utmost importance. The next set of questions relate to this RfQ-requirement._

# Q 12- Identify and explain the workings of TWO sorting algorithms and discuss and compare their performance/efficiency (i.e. Big O) 300 - 500 words

## Bubble sort

Bubble sort or sinking sort is one of the oldest sorting algorithms in computer science. It works by comparing adjacent element and swaps them if needed. Bubble sort will iterate over a list repeatedly until the list is sorted. It gets its' name from the way the elements (small or large) "bubble" to the top. 

**PROS**  
- Under a best-case scenario bubble sort has a constant complexity of 0(n). 
- Bubble sort has been used for many years and is easy to understand, therefore making it an attractive sorting method
- Does not use large amounts of memory
- Though considered inefficient compared with other sorting algorithms the difference is not significant for 100 items or less.


**CONS**-
- Bubble sort is considered to be the least efficient sorting algorithm when compared to other sorting algorithms and has a 0(n2) complexity in a worst-case scenario.

REFERENCES

https://study.com/academy/lesson/sorting-algorithm-comparison-strengths-weaknesses.html

https://en.wikipedia.org/wiki/Bubble_sort

https://en.wikipedia.org/wiki/Sorting_algorithm#Bubble_sort

## Merge sort

Merge sorting is another sorting algorithm that uses a divide-and-conquer method when sorting items. This is done by breaking down a list of items into sub-lists until there is only one element in each list and then merging all sub-lists into a single sorted list.

**PROS**
- Under a worst-case scenario merge sort has a complexity of 0(n log n) which makes it an efficient sorting algorithm when compared to others such as bubble sort.

- can be efficiently applied for files of any size

**CONS**
- Requires more space than bubble sort as there needs to be space reserved for the sub-lists

REFERENCES

https://www.glassdoor.com/Interview/Pros-cons-of-merge-sort-and-quick-sort-QTN_1769819.htm

https://www.quora.com/What-are-the-pros-and-cons-of-merge-sort

https://study.com/academy/lesson/sorting-algorithm-comparison-strengths-weaknesses.html 

# Q 13- Identify and explain the workings of TWO search algorithms and discuss and compare their performance/efficiency (i.e. Big O) 300 - 500 words

## Binary Search

When searching an array binary search will divide the array in half. If the value being searched for is higher than the middle value then the lower half is discarded and the top half is used to search for the value. The same is performed if the value is lower than the middle then the top half is discarded and only the lower half is searched. Finally, if the value is equal to the middle element then the middle index is returned. To best implement binary search typically two prerequisites must be met: the items should be in sorted order and random elements can be accessed in constant time.

**PROS**
- In a worst-case scenario binary search has a complexity of 0(log n) this makes it an efficient and scalable sorting algorithm 

- Efficient for large datasets

**CONS**
- Although binary search is good for large datasets but performing binary search on linked lists will have the same time complexity as a linear search (0(n) in a worst-case scenario). This is because items in a linked list cannot be accessed in constant time.

- For best implementation items should be sorted and random elements can be accessed in constant time.

## Linear Search

Linear search is very simple algorithm used to find an element in a list. A linear search algorithm will look for an element in a list by sequentially moving through the list. 

**PROS**
- Linear search has a 0(n) complexity and is good for small datasets
- Linear search is very basic algorithm and easy to implement
- Linear search is also memory efficient and doesn't require copying for memory allocation

**CONS**
- Not efficient when using large datasets
- This algorithm scales linearly

REFERENCES
https://www.quora.com/Why-is-binary-search-not-possible-using-linked-list

https://www.geeksforgeeks.org/binary-search/

https://www.geeksforgeeks.org/linear-search/

https://en.wikipedia.org/wiki/Linear_search

https://en.wikipedia.org/wiki/Binary_search_algorithm#Binary_search_versus_other_schemes

https://peterstratton.com/posts-output/2017-02-09-linear-search/

_Companies (including ACME Corporation) value previous project experience and case studies. The following set of questions relate to this RfQ-requirement._

# Q14 - Conduct research into a marketplace website (app) and answer the following parts:  

  a. List and describe the software used by the app.
  
  b. Describe the hardware used to host the app.

  c. Describe the interaction of technologies within the app

  d. Describe the way data is structured within the app

  e. Identify entities which must be tracked by the app

  f. Identify the relationships and associations between the entities you have 
  identified in part (e)
  
  g. Design a schema using an Entity Relationship Diagram (ERD) appropriate for the database of this website (assuming a relational database model)