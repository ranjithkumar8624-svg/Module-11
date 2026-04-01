# 📝 Singly Linked List: Add Element at the Start

This Python program demonstrates the implementation of a **Singly Linked List** where a new element can be added at the **start** of the list.

---

## 🎯 Aim

To write a Python program that adds a **new element** at the **start** of a singly linked list. The program implements a `push_front` method that inserts an element at the front of the list, followed by a method to print the list.

---

## 🧠 Algorithm

1. **Step 1:** Define a class `Node` with:
   - `data` to store the node's value.
   - `next` to store the reference to the next node.
   
2. **Step 2:** Define a class `LinkedList` with:
   - `head` to point to the first node.
   
3. **Step 3:** In the `LinkedList` class, define a method `push_front(newElement)`:
   - Create a new node with `newElement`.
   - Set the new node's next pointer to the current head node.
   - Set the head to the new node.

4. **Step 4:** Define a method `PrintList()` to display the list:
   - Print the elements of the list or display "The list is empty." if the list is empty.

5. **Step 5:** Instantiate a `LinkedList` object, `MyList`, and add elements at the start using the `push_front()` method.

6. **Step 6:** Call the `PrintList()` method to display the list.

---

## Program
class Node:
def init (self, data):
self.data = data
self.next = None
class LinkedList:
def init (self):
self.head = None
def push(self, new_data):
new_node = Node(new_data)
new_node.next = self.head
self.head = new_node
def search(self, x):
current = self.head
while current:
if current.data == x:
return True
current = current.next
return False
llist = LinkedList()
llist.push(10);
llist.push(30);
llist.push(11);
llist.push(21);
llist.push(14);
data = int(input())
if llist.search(data):
print("Yes")
else:
print("No")
## Sample Output
<img width="276" height="148" alt="image" src="https://github.com/user-attachments/assets/db749a17-4d5c-4859-9fc6-5ddbcff816d0" />

## Result

Thus the program was executed successfully
