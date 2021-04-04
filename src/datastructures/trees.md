# Trees

Trees in Computer Science is reversed to what we know. The Root sits at the top, while the leaves are in the bottom.

On a more technical definition:
A tree is a collection of entities called nodes. Nodes are connected by edges. Each node typically contains a value and it may or may not have a child node. Tree nodes are 1 or more of the following:
* Root - The start of the tree, visualised at the top.
* Parent - A parent node, connecting to atleast 1 or more children.
* Child - A child node, has exactly one parent.
* Leaf node - A leaf node is one that does not have any children.

# Binary Trees(BT)

A Binary Tree is a tree data structure in which each node has at most two children, which are referred to as the left child and the right child. 
Binary trees are often used to solve problems efficienctly. 

# Binary Search Trees(BST)
A Binary Tree with an extra property:
The right child is always greater or equal to the parent whilst the left child is always less than the parent.
Let's look at an example:

![image](https://user-images.githubusercontent.com/32796571/113524372-7da8e180-95ae-11eb-96eb-66efb25aea2d.png)

As we can see, this is the tree form. Root on top, parents connected to their childs. Binary tree property that each node has up to two children.
Finally, we see the important property of Binary Search Trees: the parent is always greater than it's left child and less or equal to it's right child (ex. 17 > 16, 17 <= 20).

So how is this property used? Very simply, to efficiently search for a specific value in the datastructure. If we are looking in our example for 16, we set the current to the root and we keep traversing based on whether our desired destination is smaller or larger than the current.
Hence, looking for 20 would be done in the following steps:
1. Root is 13, current is 13.
2. 13 is less than 20, go right. Current -> 23
3. 23 is more than 20, go left. Current -> 17
4. 17 is more than 16, go right. Current -> 16
5. Current is 16, our desired position.

This form of search is done on average in O(log(N)) time, way faster than linearly searching through them. This of course relies on the balance of the tree, as in the worst case, the Tree ends up being a Linked List and searching through is O(n).

Implementation:

For implementation advice, I would suggest to brush up on pointers and look at Exercise 8 solutions whilst keep visualising the steps on a BST.

Red Black Trees:

Self Balancing Binary search Trees, guarantee a search performance of O(log(n)). Look at slides for more detailed explanation.

