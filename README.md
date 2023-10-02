# CMU-15-721
To become a better engineer I'm taking the Carnegie Mellon University course 15-721 (Advanced Database Systems) to learn OLAP/OLTP engineering. I have a personal interest in high performance computing and there are many crossovers between that and the subjects taught in this course, such as kernel bypass methods (low latency networking), parallel processing, multithreading, cache management and more which I will be learning.

Prof Andy Pavlov teaches this course and he is incredibly knowledgable on the subject. The lectures can be found on youtube here: https://www.youtube.com/watch?v=LWS8LEQAUVc&list=PLSE8ODhjZXjYzlLMbX3cR0sxWnRM7CLFn

### Lecture 4 - Analytical Database Indexes
This lecture focuses on how to optimize sequential scans on a database. 

I learned about Zone Maps, which are essentially storing metadata inside a memory block which contains common aggregate data that might be queried often, like MIN, MAX, AVG, SUM and COUNT. This reduces the time complexity of scanning to O(1) in the case where you need the aggregate data.

I also learned about Bit Weaving, which allows you to store your indexes as bit vectors in such a way that you can take advantage of bitwise operations to very efficiently check if the data you need is in the memory block.

### Bloom Filters
One of the data structures mentioned in this course is the Bloom Filter. The Bloom Filter is a "probabalistic data structure". This interested me because I had never heard of it before, so I decided to make my own implementation. You can see the video here on Youtube: https://youtu.be/I2p2Zpir-9c?si=iX7oVQ3f8FcDfmzU
