#BINARY TREES
in this project, we explored the data structure, Binary Tree-a hierarchical and non-linear data structure which finds application in areas like binary search tree, application that make use of hierarchy etc. The following data structures and types for binary trees were used in this project.

#Basic Binary tree
```/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;```

##Binary Search tree
```typedef struct binary_tree_s bst_t;```
##AVL Tree
```typedef struct binary_tree_s avl_t ;```
##Max Binary Heap
```typedef struct binary_tree_s heap_t;```

##Print Function
 the print function found [here](https://github.com/alx-tools/0x1C.c) was used for the pretty visualization of the output of the tasks implemented
 
 ##Tasks
 * [0-New Node](./0-binary_tree_node.c)
 function that creates a binary tree node using the prototype ```binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);```. `parent` is the pointer to the parent node, `value` is the data stored in the node. return pointer to the new node or `NULL` on failure
 
 * [1. Insert left](./1-binary_tree_insert_left.c)
 Insert left child node, becomes the left child of the given parent while the previous left child(if any) becomes the left child of the node created. prototype is ```binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);```
 
  * [2. Insert left](./2-binary_tree_insert_right.c)
 Insert right child node, becomes the right child of the given parent while the previous right child(if any) becomes the right child of the node created. prototype is ```binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);```
 
 *[3. Delete](./3-binary_tree_delete)
 Delete a binary tree.
 prototype: ```void binary_tree_delete(binary_tree_t *tree);```
 
 *[4. Is Left](./4-binary_tree_is_left.c)
 Check whether the given node is a left child
 prototype: ```int binary_tree_is_leaf(const binary_tree_t *node);```
 
 *[5. Is root](./5-binary_tree_is_root.c)
 Check whether the given node is the root node.
 prototype: ```int binary_tree_is_root(const binary_tree_t *node);```
 
 *[6. Pre-order traversal](./6-binary_tree_preorder.c)
 Traverse a binary tree using pre-order traversal.
 prototype: ```void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));```
 
 *[7. In-order traversal](./7-binary_tree_inorder.c)
 Traverse a binary tree using in-order traversal.
 prototype: ```void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));```
 
 *[8. Post-order traversal](./8-binary_tree_postorder.c)
 Traverse a binary tree using post-order traversal.
 prototype: ```void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));```
 
 *[9. Height](./9-binary_tree_height.c)
 Measure the height of  a binary tree
 prototype: ```size_t binary_tree_height(const binary_tree_t *tree);```
 
 *[10. Depth](./10-binary_tree_depth.c)
 Measure the depth of a node in a binary tree
 prototype: ```size_t binary_tree_depth(const binary_tree_t *tree);```
 
 *[11. Size](./11-binary_tree_size.c)
Measure the size of a binary tree
prototype: ```size_t binary_tree_size(const binary_tree_t *tree);```

*[12. Leaves](./12-binary_tree_leaves.c)
Count leaves in a binary tree
prototype: ```size_t binary_tree_leaves(const binary_tree_t *tree);```

*[13. Nodes](./13-binary_tree_nodes.c)
Node with atleast 1 child in a binary tree
prototype: ```size_t binary_tree_nodes(const binary_tree_t *tree);```

*[14. Balance factor](./14-binary_tree_balance.c)
Measure the balance factor of a binary tree.
prototype: ```int binary_tree_balance(const binary_tree_t *tree);```

*[15. Is full] (./15-binary_tree_is_full.c)
Check if a binary tree is full
prototype: ```int binary_tree_is_full(const binary_tree_t *tree);```

*[16. Is perfect](./16-binary_tree_is_perfect.c)
Check if binary tree is perfect
prototype: ```int binary_tree_is_perfect(const binary_tree_t *tree);```

*[17. Sibling](./17-binary_tree_sibling.c)
Find the sibling of a given node.
prototype: ```binary_tree_t *binary_tree_sibling(binary_tree_t *node);```

*[18. Uncle](./18-binary_tree_uncle.c)
Find the uncle of a given node.
prototype: ```binary_tree_t *binary_tree_uncle(binary_tree_t *node);```
	
*[19. Lowest common ancestor](./100-binary_tree_ancestor.c)
Find the lowest common ancestor of two given nodes.
prototype: ```binary_tree_t *binary_trees_ancestor(const binary_tree_t *first, const binary_tree_t *second);```

*[20. Level order traversal](./101-binary_tree_level_order.c)
Traverse a binary tree using level order traversal.
prototype: ```void binary_tree_levelorder(const binary_tree_t *tree, void (*func)(int));```
	
*[21. Is complete](./102-binary_tree_is_complete.c)
Check if a binary tree is complete.
prototype: ```int binary_tree_is_complete(const binary_tree_t *tree);```

*[22. Rotate left](./103-binary_tree_rotate_left.c)
Performs left rotation on a binary tree.
prototype: ```binary_tree_t *binary_tree_rotate_left(binary_tree_t *tree);```
	
*[23. Rotate right](./104-binary_tree_rotate_right.c)
Performs right rotation on a binary tree.
prototype: ```binary_tree_t *binary_tree_rotate_right(binary_tree_t *tree);```
	
*[24. Is BST](./110-binary_tree_is_bst.c)
Check if a binary tree is a valid Binary Search Tree (BST).
prototype: ```int binary_tree_is_bst(const binary_tree_t *tree);```

*[25. BST insert](./111-bst_insert.c)
Insert a value in a BST.
prototype: ```bst_t *bst_insert(bst_t **tree, int value);```

*[26. BST - Array to BST](./112-array_to_bst.c)
Builds BST from an array.
prototype: ```bst_t *array_to_bst(int *array, size_t size);```

*[27. BST - Search](./113-bst_search.c)
Searches for a value in a BST.
prototype: ```bst_t *bst_search(const bst_t *tree, int value);```
	
*[28. BST - Remove](./114-bst_remove.c)
Removes a node from a BST.
prototype: ```bst_t *bst_remove(bst_t *root, int value);```
	
*[29. Big O #BST](./115-0)
Contains the Big O per line of the following operations on BST.
	** Insert the value n
	** remove the node with the value n
	** search for a node in a BST of size n

*[30. Is AVL](./120-binary_tree_is_avl.c)
Check if a binary tree is a valid AVL tree.
prototype: ```int binary_tree_is_avl(const binary_tree_t *tree);```
	

*[31. AVL - Insert](./121-avl_insert.c)
Insert a value in an AVL tree.
prototype: ```avl_t *avl_insert(avl_t **tree, int value);```
	
*[32. Array to AVL](./122-array_to_avl.c)
Builds an AVL tree from an array.
prototype: ```avl_t *array_to_avl(int *array, size_t size);```
	
*[33. Remove](./123-avl_remove.c)
Removes a node from an AVL tree.
prototype: ```avl_t *avl_remove(avl_t *root, int value);```
	
*[34. AVL - from sorted array](./124-sorted_array_to_avl.c)
Builds an AVL tree from an array.
prototype: ```avl_t *sorted_array_to_avl(int *array, size_t size);```
	
*[35. Big O # AVL Tree](./125-0)
Contains the Big O per line of the following operations on AVL.
	** Insert the value n
	** remove the node with the value n
	** search for a node in a BST of size n
	
*[36. is Binary Heap](./130-binary_tree_is_heap.c)
Check if a binary tree is a valid Max Binary Heap.
prototype: ```int binary_tree_is_heap(const binary_tree_t *tree);```
	
*[37. Heap - Insert](./131-heap_insert.c)
Inserts a value in Max Binary Heap.
prototype: ```heap_t *heap_insert(heap_t **root, int value);```
	
*[38. Heap - Array to Binary Heap](./132-array_to_heap.c)
Builds a Max Binary Heap tree from an array.
prototype: ```heap_t *array_to_heap(int *array, size_t size);```
	
*[39. Heap - Extract](./133-heap_extract.c)
Extracts the root node of a Max Binary Heap.
prototype: ```int heap_extract(heap_t **root);```
	
*[40. Heap - Sort](./134-heap_to_sorted_array.c)
Converts a Binary Max Heap to a sorted array of integers.
prototype: ```int *heap_to_sorted_array(heap_t *heap, size_t *size);```
	
*[41. Big O #Binary Heap](./135-0)
Contains the Big O per line of the following operations Binary Heap.
	** Insert the value n
	** Extracting the root node
	** search for a node in a binary heap of size n
