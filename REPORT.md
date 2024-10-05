> Oct 4, 2024          
> Samrat Baral
> Student ID #005030064

> MSCS532 Algorithms and Data Structures - First Bi-term

> Assisgnment 7

---

# Hash Table Key Concepts and Strategies 

## Introduction:

Hash Table is an data structure which behavies like a dictonary using key-value pairs mapping those data for insertion, update and deletion. Hashing concept was credited to Arnold Dumey, who discussed the idea of using remainder modulo a prime as a hash function. therefore sometime hashing algorithms prefer to have the size be a prime number. In computers language its an associative array which stores a set of (key, value) pairs and allows insertion, deletion, and lookup (search), with the constraint of unique keys. It requirs to have uniform distribution for hashing function else it will increase the complexity and collison cost.(GeeksforGeeks) A hash table’s load factor is determined by  size of relation,  hash function and  proper table resizing. The table may be cluttered that's why the hash function should avoid clustering becaue it causes high lookup cost, even though the load factor is low and collisions are infrequent. So concepts like open addressing mitigate and avoid clustering. Therefore, A search algorithm that uses hashing consists of has part for key into an array index and other for collision resolution. (Wikipedia)

### 1. Hash Functions and Their Impact:

#### **Designing Effective Hash Functions:** 

Hash functions play a critical role in determining the efficiency of a hash table by giving them keys and array indices is known as a hash function. A good hash function have effiecient computing and uniformly distribute the keys. If its done correctly it is called  perfect hash function (Geeksforgeek). Most pratical usage of hash function is with  heuristic techniques which include division and multiplication. It has found that the best results with the division method are achieved when the table size is prime. If many keys can have the same hash then it cause collision.To mitigate the issue we keep it uniformly distrubuted the key which meant to keep hashing and key constant. Hence its crucial for hashing function to operate the hashing effieceintly. so, its hard to read hash value rather uts good practise to attempt to guess the key using the hash value rather than retriving the original hash. Thus hashing functions should be flexible as data is changed or the formating scheme changes. 

#### **Balancing Speed and Complexity:** 

We know now that hashing has efficent and effective if the hash function are uniformly distrubuted and the keys hash are on table without collison. There are some factor that might affect real-world scenarios that need trade-offs involved in designing hash functions that are both computationally efficient and resistant to collisions. In hash table it can frequently use the information with o(1) time which is rapid access. The time complexity of O(1) on avergae case for insertion, deletion and udpate but  worse case is O(n) which due to larger data of n size elements.  When more or equal to two keys have the same hashing then there occure collision that impact the speed and complexity of the application. There are technique such as open addressing or as open hashing, close hashing or know as seperate chaining and robin Hood hashing. 


### 2. Open Addressing vs. Separate Chaining:

#### **Comparing Collision Resolution Strategies:** 

Open addressing and separate chaining are two primary methods for handling collisions in hash tables as we know from above lets discuss more about its techniques. seperate chaining adding the collided element to the linklist and adding the new key on it. why its done so? its due to the fact that sometimes its unknow how many key it requires when collision happened. some practical, such as a password storage system, a slower, cryptographic hash function is essential to ensure data security, whereas for a caching mechanism where speed is critical, a faster hash function with acceptable collision rates is more suitable. which method is correct then we might have to consider memory constraints, dataset flexibity,and average vs. worst Case: In applications like caching or dictionaries, where average-case performance is critical, separate chaining can often provide more consistent access times.

#### **Performance in Practice:** 
Assembling the chain structure insures the hash table never full or need more elements. but the performance might be increase due increase complexity and space but really simple to implement. Similarly open-addressing but different implentation which insures collision-resolution keeping in the hash table contact with size is never equal to or less than the number of keys present. Linear, double and quadratic hasshing are techniques to mitigate collisions. In comparison to linear probing, quadratic probing has a worse cache performance eventhought clustering is less of a concern with quadratic probing where as linear have the clustering issue and time to find hte empty slot is incremental which happends in the iterative for empty slot. Double hashing is basically hashing twice it can make time complexity increase while impling more space required. Conversely, separate chaining maintains efficient average-case performance regardless of the load factor, provided that the underlying list is well-managed.

## Conclusion

Hash tables are vital for efficient data retrieval, relying on effective hash functions and collision resolution strategies. Good hash functions ensure uniform distribution and minimize collisions, while open addressing and separate chaining offer different approaches to handle collisions, each with unique advantages depending on memory constraints and data characteristics. In summary, understanding the intricacies of hash functions and collision resolution methods is crucial for optimizing hash table performance in various applications. By selecting appropriate strategies, developers can enhance efficiency and reliability, ensuring that hash tables meet the demands of diverse real-world scenarios effectively.


## References:

“Hash Table Data Structure.” GeeksforGeeks, GeeksforGeeks, 15 Sept. 2024, www.geeksforgeeks.org/hash-table-data-structure/. 

“What Are Hash Functions and How to Choose a Good Hash Function?” GeeksforGeeks, GeeksforGeeks, 21 Feb. 2023, www.geeksforgeeks.org/what-are-hash-functions-and-how-to-choose-a-good-hash-function/. 

“Hash Table.” Wikipedia, Wikimedia Foundation, 27 Sept. 2024, en.wikipedia.org/wiki/Hash_table. 

“Collision Resolution Techniques.” GeeksforGeeks, GeeksforGeeks, 5 Apr. 2024, www.geeksforgeeks.org/collision-resolution-techniques/. 