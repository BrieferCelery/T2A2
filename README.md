## Workbook - Aaron Kane
# Q1 - Describe the architecture of a typical Rails application

Rails architecture follows the Model-View-Controller(MVC) design pattern where the major components of the application are organised into three layers in order to achieve a "separation of concerns". This separation of concerns increases the application's robustness and testability as each component has no knowledge of the other.

## The model
The model is the application's data structure and has no knowledge of the user interface. It handles the data logic for the rails application. The model layer communicates with the database and makes it available through the controller. The model is typically located in the app/model folder.

## Controller
The controller layer is the mediator between the model and the view and controls the flow of the application. In a typical rails application the controller will query the database and organise it in order to pass it to the view.

## view
The view represents the data to the user. In a rails application this is typically done with embedded ruby or haml. Rails views are typically located in the app/views folders.


## Diagram of a typical rails application
![](rails_mvc.png)
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


# Q3 - Discuss the implementation of Agile project management methodology
Agile project management is methodology for delivering projects based on iteration. Agile can also be considered a mindset that can respond to ever changing requirements of the project. Agile has become a popular mothodology worldwide for project management as there are numerous advantages to this approach. Firstly, agile is implemented using the scrum flow where teams deliver products in short cycles as opposed to one delivery at the end of a project. Agile is focused on user feedback. User feedback is essential in agile development as iterations are made to the product based on such feedback. The feedback is documented and placed in the backlog. Another advantage to using the agile approach is user stories. User stories give developers insight into client needs by putting the end user at the centre of feature development. User stories typically contain a brief description of the needs of the user for example - "as a user I should be able to register an account". After completing these features feedback from end client is tested to guage customer satisfaction. Agile can also be seen as a mindset where teams must have a flexible mindset in order to respond accordingly to changing demands of a project.

REFERENCES

https://www.visual-paradigm.com/guide/agile-software-development/what-is-user-story/

https://www.guru99.com/waterfall-vs-agile.html



# Q4 - Provide an overview and description of a standard source control workflow

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





# Q 13- Identify and explain the workings of TWO search algorithms and discuss and compare their performance/efficiency (i.e. Big O) 300 - 500 words
