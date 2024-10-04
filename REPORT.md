> Oct 4, 2024          
> Samrat Baral
> Student ID #005030064

> MSCS532 Algorithms and Data Structures - First Bi-term

> Assisgnment 7

---

# Hash Table Key Concepts and Strategies 

## Introduction:

Hash Table is an data structure which behavies like a dictonary using key-value pairs mapping those data for insertion, update and deletion. Hashing concept was credited to Arnold Dumey, who discussed the idea of using remainder modulo a prime as a hash function. therefore sometime hashing algorithms prefer to have the size be a prime number. In computers language its an associative array which stores a set of (key, value) pairs and allows insertion, deletion, and lookup (search), with the constraint of unique keys. It requirs to have uniform distribution for hashing function else it will increase the complexity and collison cost. A hash table’s load factor is determined by  size of relation,  hash function and  proper table resizing. The table may be cluttered that's why the hash function should avoid clustering becaue it causes high lookup cost, even though the load factor is low and collisions are infrequent. So concepts like open addressing mitigate and avoid clustering. Therefore, A search algorithm that uses hashing consists of has part for key into an array index and other for collision resolution. 

### 1. Hash Functions and Their Impact:

#### **Designing Effective Hash Functions:** 

Hash functions play a critical role in determining the efficiency of a hash table by giving them keys and to array indices is known as a hash function 


Hash Table determine
Discuss the characteristics of a good hash function and how it affects the performance of a hash table.


Provide examples of situations where poor hash function design led to performance issues such as clustering or high collision rates. 

How can these issues be mitigated?

#### **Balancing Speed and Complexity:** 

Hash functions need to be both fast and effective at distributing keys uniformly. Discuss the trade-offs involved in designing hash functions that are both computationally efficient
and resistant to collisions. Provide a case study or example to illustrate how these trade-offs impact real-
world applications.


### 2. Open Addressing vs. Separate Chaining:

#### **Comparing Collision Resolution Strategies:** 
Open addressing and separate chaining are two primary methods for handling collisions in hash tables. Compare these two strategies in terms of their efficiency, memory usage, and complexity. In what scenarios would one be preferred over the other? Provide examples from real-
world applications to support your discussion.

#### **Performance in Practice:** 

Analyze how open addressing performs under different load factors compared to
separate chaining. Discuss the practical considerations, such as memory constraints and the nature of the data, that influence the choice between these methods in a given application.

## References:

“Hash Table Data Structure.” GeeksforGeeks, GeeksforGeeks, 15 Sept. 2024, www.geeksforgeeks.org/hash-table-data-structure/. 

“Hash Table.” Wikipedia, Wikimedia Foundation, 27 Sept. 2024, en.wikipedia.org/wiki/Hash_table. 