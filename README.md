# udacity_dsa2
Udacity coursework - data structure

### Problem 1: LRU Cache
#### 1.Code Design:

LRU is designed to get and store the recent value with first priority.
Python Dictionary (from Python 3.10 onward) stores value in order of recent action. So, Dictionary is used to design storage of LRU.

#### 2.Efficiancy:

Time complexity: Overall is O(1). All process can be done with single run such as store information into dictionary or get information from dictionary.
- (1) To get value is O(1)
- (2) To set value is O(1)

Space complexity:
depend on "capacity", which is defined by user.

-------------

### Problem 2: File Recursion
#### 1.Code Design:

Recusion is used to implemented find_file function because it has capability to continue process until reaching the edge without knowing the limitation at the beginning stage.

#### 2.Efficiancy:

Time complexity: O(n) because it depends on number of file and level of directory to go through. 
- O(n), n is number of files and level of directory.

Space complexity: depend on number of files in the considered directory

-----------

### Problem 3: Huffman Coding
#### 1.Code Design:

Node with tree structure is used to store information of Huffman Coding, which it has ability to record key (string), value (frequency). The parent node of child is summation of their child frequency. It can also encode value of the edge of child.

#### 2.Efficiancy:

Time complexity: Overall, the time complexity is O(n), which n is number of node.
- (1) Methods of Node and Tree is O(1).
- (2) find_frequency() is O(n) from collections.Counter().
- (3) insert_node() is O(n) from for-loop to go through all node list.
- (4) build_tree() is O(n) from while-loop to go through all node list.
- (5) tree_encoder() is O(n) from recusion.
- (6) decoder() is O(n) from recusion.
- (7) huffman_decoding() is O(n) from while-loop.

Space complexity:
depend on number of string of text.

------------

### Problem 4: Active Directory
#### 1.Code Design:

List is used to store information of groups and users. It also provides straightforward tool to add new information to the list.

#### 2.Efficiancy:

Time complexity: Overall, the time complexity is O(1) and O(n), which n is number of user and group.
- O(1) when to add user or group.
- O(n) because it depends on number of group. and users.

Space complexity: depend on number of user and group.

-------------

### Problem 5: Blockchain
#### 1.Code Design:

Linked list is chosen to implement to build blockchain. It provides ability to store information of previous node which is linked.

#### 2.Efficiancy:

Time complexity: O(1) when to add new block.
Space complexity: depend on number of block.

-------------

### Problem 6: Union and Intersection
#### 1.Code Design:

Python List is selected to implement as it has an ability to union and intersect data.
List of Node is firstly converted to List. Then do union or intersect. Finally, it is converted back to Node list.

#### 2.Efficiancy:

Time complexity: Overall time complexity is O(n) + O(n log n), which n is number of node.
- (1) collect_node(llist) is O(n) - it goes though list of Node.
- (2) union is O(n) + O(n log n). O(n log n) is from union, O(n) is from loop ton convert from list to Node list.
- (3) intersection is O(n) + O(n log n). O(n log n) is from intersect, O(n) is from loop ton convert from list to Node list.

Space complexity: depend on number of node.



