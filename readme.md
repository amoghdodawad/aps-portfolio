# Algorithmic problem solving portfolio
 - **Course Name:** Algorithmic Problem Solving
 - **Course Code:** 23ECSE309
 - **Name:** Amogh Shrikant Dodawad
 - **University:** KLE Technological University, Hubballi-31

---

# Overview
This portfolio explores and analyses the functionalities provided by OTT platforms along with the algorithms used to implement the respective funtionalities along with their time and space efficiency.

# Table of contents
1. [Introduction](#introduction)
2. [Objectives](#objectives)
3. [Functionalities](#functionalities)
4. [Efficiency analysis](#efficiency-analysis)
5. [References](#references)

# Introduction
OTT platforms have been some of the most revolutionary services saw the light of the day with the advent of internet.
    The un-matched flexibility provided by the OTT platforms ensured that they became very popular in very less time, hence, the scale, which is good from a business PoV, is a rather difficult task when looked at from a engineering PoV, became a critical thing to handle. Thus making sure that right components are used in the right manner are critical to ensuring the scalabilty in service offerings. One of these components are the algorithms used in designing these services. This portfolio explores how algorithms made OTTs what they are today.

# Objectives
- Identify and analyze existing OTT platform functionalities.
- Propose new functionalities to enhance the domain.
- Explore business use cases, challenges, and benefits.
- Suggest suitable algorithms and design techniques.

# Functionalities
1. **Adaptive bitrate streaming**
    - ![Adaptive Bitrate Streaming](abr.jpg)


    - ABR refers to the process of supporting multiple video/audio resolutions to choose from and optionally, switching between multiple resolutions based on the user's available bandwidth.
    - Few of the popular ABR algorithms/protocols are MPEG-DASH, HLS etc.
2. **Typeahead search**
    - Typeahead search refers to the functionality where the user types a part of the query he/she is intending to search and the potential list of completed queries is prompted back to the user to choose from.
    - Trie is a popular data structure to perform operations on dictionary like functionalities. This can be used in conjuction with algorithms like BFS, DFS to find the k-nearest words.
3. **Timestamps / Chapters**
    - Timestamps/chapters are the key-moments in a video where an important subject is being streamed. Allowing users to skip directly to the timestamps results in saving huge amount of bandwidth and time.
    - Algorithms like max-sum sliding-window would help in identifying the key moments in the video. Caching those results using data structures like hash-tables will greatly reduce the latency.
4. **Most-watched / Most-replayed**
    - This features enables users to look at the most viewed segments in a given video. This is a constantly changing parameter as the watch time of individual user keeps on changing as per their requirements.
    - This is more useful to the content creator as they can retrospect on their content and watch-behaviour of their users.
    - Data structures like Fenwick trees, Segment trees can optimise the process of generating this analytics.
5. **Personalised recommendation system**
    - This feature enables users to get recommendations based on their watch history and the preferences as suggested by the user himself/herself.
    - Machine learning algorithms/techniques like deep learning, NLP etc. can be used to effectively generate the personalised feed for each user.
6. **Multi-parameter filtering**
    - This feature enables users to filter the content based on multiple parameters like genre, language, year etc.
    - Data structures like BST, B-trees help in effectively filtering the content.
    - Data structures like Union-find help in identifying the similar filters to ones provided by the user.
7. **Pagination**
    - This feature enables user to view top-k suggestions in their personalised feed at a time.
    - This is highly important for the server and the database as well, as querying and processing a large chunk of data is highly resource intensive.
    - Data structures like heaps are highly efficient in sorting out of the top-k suggestions.


# Efficiency analysis

| **Algorithm**                         | **Time Complexity**                            | **Space Complexity**                          |
|---------------------------------------|------------------------------------------------|-----------------------------------------------|
| **Segment Trees**                     | Build: O(n log n), Query/Update: O(log n)      | O(n)                                          |
| **Red-Black Trees**                   | Insert/Delete/Search: O(log n)                 | O(n)                                          |
| **Binary Search Tree**                | Insert/Delete/Search: theta(log n), O(n)       | O(n)                                          |
| **Dijkstra's Algorithm**              | O((V + E) log V)                               | O(V^2)                                        |
| **A* Search Algorithm**               | O(E)                                           | O(E)                                          |
| **Trie Data Structure**               | Insert/Search: O(n)                            | O(n) each node                                |
| **B Trees**                           | Insert/Delete/Search: O(log n)                 | O(n)                                          |
| **Hash Tables**                       | Insert/Delete/Search: theta(1), O(n)           | O(n)                                          |
| **BFS and DFS**                       | O(V + E)                                       | O(V)                                          |
| **Union-Find**                        | Union/Find: O(α(n))                            | O(n)                                          |
| **Topological Sorting**               | O(V + E)                                       | O(V)                                          |
| **Kruskal's Algorithm**               | O(E log E)                                     | O(E + V)                                      |
| **Heap Data Structure**               | Insert/Delete/Extract-Min: O(log n)            | O(n)                                          |
| **Fenwick Trees**                     | Build: O(n log n), Update/Query: O(log n)      | O(n)                                          |
|---------------------------------------|------------------------------------------------|-----------------------------------------------|

# References
