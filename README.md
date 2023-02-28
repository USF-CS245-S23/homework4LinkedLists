# Homework 4: Singly Linked Lists

In this homework, you will practice working with custom singly linked lists. You will need to implement four methods:

- LinkedList sublist(int value1, int value2)

This method should return a sublist of the given list where the values of elements are in the range from value1 to value2, inclusive.
Example:
If the list is 6->40->3->17->1 and value1 is 3 and value2 is 20, then the result should be 6->3->17.
Note: Your method should not destroy the original list and its nodes should *not* reference the nodes in the input list, you need to create new nodes instead.

- public void insertInSortedList(int elem) 

The method should insert a new node with the given element into the sorted linked list. It should insert it in the right place based on the value in the node. 
Assume the list is sorted by the elem, from smallest to largest. 
The list should remain sorted after this insert operation. 

Example: If this list is 5->10->18 and we insert 15, then after that the operation,
the list will become 5->10->15->18.

- LinkedList getKLargest(int k)

Assume a singly linked list is sorted in ascending order, and we do not know the number of elements. The method should return a LinkedList that contains k largest elements in the list.
You are required to use slow & fast pointers to find the k-th node from the end as we discussed in class. 
Note: This method should be linear and should not count the number of nodes. Do NOT use reverse(). You may use the provided append method to add nodes to the new list.

Example: if the list is 4->10->12->40->55 and we call getKLargest(3), the method should return 12->40->55.

- static LinkedList mergeSortedLists(LinkedList list1, LinkedList list2) 

The method should merge two sorted linked lists into a single sorted linked list (in ascending order). Do not destroy the given lists.
You may use the provided append method to add nodes to the new list.

Example: if list1 is 1->5->11, and list2 is 2->3->10->22, then the result should be 1->2->3->5->10->11->22.

The instructor provided the tests for this homework (see Homework4Test file), but passing these basic tests does not guarantee that your code is correct. You are responsible for doing additional testing.
