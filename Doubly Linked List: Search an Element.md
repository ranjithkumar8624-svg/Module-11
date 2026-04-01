# 📝 Doubly Linked List: Search an Element

This Python program demonstrates the implementation of a **Doubly Linked List** where you can insert elements at both the beginning and the end of the list. Additionally, it allows you to search for a specific element in the list.

---

## 🎯 Aim

To write a Python program that:
- Implements a **Doubly Linked List** with functions to insert elements at the beginning and the end of the list.
- Implements a search function to check if a given element exists in the list.

---

## 🧠 Algorithm

1. **Step 1:** Define a class `Nodeq` with:
   - `data` to store the node's value.
   - `next` to store the reference to the next node.
   - `prev` to store the reference to the previous node.

2. **Step 2:** Define a class `DoublyLinkedList` with:
   - `head` to point to the first node.

3. **Step 3:** In the `DoublyLinkedList` class, define methods:
   - `insert_beginning(data)` to insert a node at the beginning.
   - `insert_end(data)` to insert a node at the end.
   - `search(data)` to search for an element in the list.

4. **Step 4:** Create an instance of `DoublyLinkedList`.
   - Insert elements at the beginning and end.
   - Search for specific elements.

---

## 💻 Program
class Node: def init(self, my_data): self.previous = None self.data = my_data self.next =
None class double_list: def init(self): self.head = None self.tail = None def add_data(self,
my_data): new_node = Node(my_data) if(self.head == None): self.head = self.tail =
new_node self.head.previous = None self.tail.next = None else: self.tail.next = new_node
new_node.previous = self.tail self.tail = new_node self.tail.next = None def print_it(self):
curr = self.head if (self.head == None): print("The list is empty") return print("The nodes
in the doubly linked list are :") while curr != None: print(curr.data) curr = curr.next def
search_node(self, val_to_search): i = 1; flag_val = False; curr = self.head; if(self.head ==
None): print("List is empty") return while(curr != None): if(curr.data == val_to_search):
flag_val = True break curr = curr.next i = i + 1 if(flag_val): print("The node is present in
the list at position : ") print(i) else: print("The node isn't present in the list") my_instance
= double_list() print("Elements are being added to the doubly linked list")
my_instance.add_data(10) my_instance.add_data(24) my_instance.add_data(54)
my_instance.add_data(77) my_instance.add_data(24) my_instance.add_data(0)
my_instance.print_it() print("The element 77 is being searched... ")
my_instance.search_node(77) print("The element 7 is being searched... ")
my_instance.search_node(7)
## Sample Output
<img width="541" height="149" alt="image" src="https://github.com/user-attachments/assets/a53547d2-4543-4655-ac98-d16b9171aefa" />

## Result
Thus the program was executed successfully
