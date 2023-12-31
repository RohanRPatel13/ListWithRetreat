# ListWithRetreat

## Objectives
1. Familiarity with writing a kernel class for a new type and its kernel operations (List with the extra retreat method) using references (also known as pointers) to build a doubly-linked list of nodes.
2. Familiarity with developing and using specification-based test plans.

## The Problem
The problem is to complete and carefully test implementations of the constructor and all kernel methods defined in interface ListKernel plus the methods retreat and moveToFinish defined in interface List, by building a representation that involves a doubly-linked list of nodes using Java references.

The retreat method gives the client the ability to move backward one position at a time. The ListKernel allows only incremental forward movement; moving backward is possible only by "jumping" all the way back to the start using moveToStart. Method retreat is just the inverse of advance.

Note that retreat (and moveToFinish) can be implemented by layering, i.e., by using only the ListKernel methods and, indeed, such implementations exist in the ListSecondary class. You should know how to write that code! However, the execution time of the layered implementations is linear in the length of the left string of the list (for retreat or of the right string of the list for moveToFinish). The challenge here is to implement ListKernel and retreat and moveToFinish so all the methods take constant time, independent of the sizes of the left and right strings of the list. This is possible only by implementing all the methods directly, i.e., not by layering on an existing implementation of ListKernel but by creating an entirely new implementation that is based on a doubly-linked list data structure.
