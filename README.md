# Binary-Search-Tree
Implementation of binary trees traversal

Input:
 
Integer item

Output: 

Linked list

Data Structure: Binary tree

Algorithm:
 
Step 1. Start
 
Step 2. Structure tree with structure variables data, *lchild and rchild is initialised
 
Step 3. Main function

  Step 3.1. Assign 0 as the value of ch
   
   Step 3.2. If value of ch is not equal to 3

     Step 3.2.1. Obtain value of ch from the user

     Step 3.2.2. If value of ch is 1, call user defined function insert();

     Step 3.2.3. If value of ch is 2

       Step 3.2.3.1. Assign 0 as the value of qq

       Step 3.2.3.2. If value of root is NULL, print “The tree is not created!”

       Step 3.2.3.3. Else if value of qq is not equal to 3

        Step 3.2.3.3.1. Obtain value of qq from the user

        Step 3.2.3.3.2. If value of qq is 1, call user defined function inorder with root as its parameter

        Step 3.2.3.3.3. If value of qq is 2, call user defined function preorder with root as its parameter

        Step 3.2.3.3.4. If value of qq is 3, call user defined function postorder with root as its parameter

        Step 3.2.3.3.5. Repeat Step 3.2.3.3.

      Step 3.2.4. Repeat Step 3.2.

Step 4. Stop

Insert() function

Step 1. Read number of nodes

Step 2. Assign value of i as 0

Step 3. If value if i is less than n
 
 Step 3.1. Obtain value of item from the user
 
 Step 3.2. Call user defined function insert with item as its parameter
 
 Step 3.3. Increase value of i by 1
 
 Step 3.4. Repeat Step 3.

Insert() function

Step 1. Create a new node head

Step 2. Assign value of item to head->data

Step 3. Assign NULL value to head->lchild and head->rchild

Step 4. If value of root is NULL, then assign value of head to root

Step 5. Else

 Step 5.1. Assign root as value of ptr and 0 as value of flag
 
 Step 5.2. If value of ptr is not equal to NULL and value of flag is 0
  
  Step 5.2.1. If value of ptr->data is less than item
   
   Step 5.2.1.1. Assign value of ptr to parent
   
   Step 5.2.1.2. Assign value of ptr->rchild to ptr
  
  Step 5.2.2. If value of ptr->data is greater than item
  
   Step 5.2.2.1. Assign value of ptr to parent
   
   Step 5.2.2.2. Assign value of ptr->lchild to ptr
  
  Step 5.2.3. Else Assign 1 as value of flag
 
 Step 5.2.4. Repeat Step 5.2.

Step 5.3. If value of flag is 1
 
 Step 5.3.1. Print “Item already exist!”

Step 5.4. Else

 Step 5.4.1. If value of parent->data is lesser than item, assign value of head as parent->rchild
 
 Step 5.4.2. Else, Assign value of head to parent->lchild.

Inorder() function with root as parameter

Step 1. Assign value of root to variable ptr

Step 2. If value of ptr is not equal to NULL
 
 Step 2.1. Call function inorder with ptr->lchild as its argument
 
 Step 2.2. Print ptr->data
 
 Step 2.3. Call function inorder with ptr->rchild as its argument
 
Preorder() function with root as parameter

Step 1. Assign value of root to variable ptr

Step 2. If value of ptr is not equal to NULL
 
 Step 2.1. Print ptr->data
 
 Step 2.2. Call function preorder with ptr->lchild as its argument
 
 Step 2.3. Call function preorder with ptr->rchild as its argument

Postorder() function with root as parameter

Step 1. Assign value of root to variable ptr

Step 2. If value of ptr is not equal to NULL
 
 Step 2.1. Call function postorder with ptr->lchild as its argument
 
 Step 2.3. Call function postorder with ptr->rchild as its argument
 
 Step 2.1. Print ptr->data
