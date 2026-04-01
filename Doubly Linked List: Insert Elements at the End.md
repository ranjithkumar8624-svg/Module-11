# 📚 Doubly Linked List: Insert Elements at the End of a Doubly Linked List

This Python program demonstrates the creation and manipulation of a **Doubly Linked List** where elements can be inserted at the **end** of the list. The program also provides a method to traverse the list and display the elements.

---

## 🎯 Aim

To write a Python program that:
- Implements a **Doubly Linked List**.
- Allows insertion of elements at the end of the list.
- Provides functionality to traverse the list and display its elements.

---

## 🧠 Algorithm

1. **Step 1:** Define a class `Node` to represent each node in the doubly linked list with attributes:
   - `item` for storing the data of the node.
   - `nref` for storing the reference to the next node.
   - `pref` for storing the reference to the previous node.

2. **Step 2:** Define a class `DoublyLinkedList` with:
   - `start_node` to point to the first node of the list.

3. **Step 3:** Define methods in the `DoublyLinkedList` class:
   - `insert_in_emptylist(data)` to insert an element when the list is empty.
   - `insert_at_end(data)` to insert elements at the end of the list.
   - `traverse_list()` to traverse the list and print the elements.

4. **Step 4:** Create an instance of `DoublyLinkedList` and use the `insert_at_end()` method to insert elements into the list.

5. **Step 5:** Use the `traverse_list()` method to print the elements of the list.

---

## 💻 Program
class Node: def init(self, data): self.item = data self.nref = None self.pref = None
class DoublyLinkedList: def init(self): self.start_node = None def insert_at_start(self,
data): if self.start_node is None: new_node = Node(data) self.start_node = new_node
print("node inserted") return new_node = Node(data) new_node.nref = self.start_node
self.start_node.pref = new_node self.start_node = new_node
def traverse_list(self):
    if self.start_node is None:
        print("List has no element")
        return
    else:
        n = self.start_node
        while n is not None:
            print(n.item, " ")
            n = n.nref
def delete_at_start(self):
    if self.start_node is None:
        print("The list has no element to delete")
        return
    if self.start_node.nref is None:
        self.start_node = None
        return
    self.start_node = self.start_node.nref
    self.start_prev = None
def delete_at_end(self):
    if self.start_node is None:
        print("The list has no element to delete")
        return
    if self.start_node.nref is None:
     self.start_node = None
        return
    n = self.start_node
    while n.nref is not None:
        n = n.nref
    n.pref.nref = None
def delete_element_by_value(self, x):
    if self.start_node is None:
        print("The list has no element to delete")
        return
    if self.start_node.nref is None:
        if self.start_node.item == x:
            self.start_node = None
        else:
            print("Item not found")
        return
    if self.start_node.item == x:
        self.start_node = self.start_node.nref
        self.start_node.pref = None
        return
    n = self.start_node
    while n.nref is not None:
        if n.item == x:
            break;
        n = n.nref
    if n.nref is not None:
        n.pref.nref = n.nref
        n.nref.pref = n.pref
    else:
        if n.item == x:
            n.pref.nref = None
        else:
            print("Element not found")
new_linked_list = DoublyLinkedList() new_linked_list.insert_at_start(10)
new_linked_list.insert_at_start(5) new_linked_list.insert_at_start(18)
new_linked_list.insert_at_start(65) new_linked_list.insert_at_start(50)
new_linked_list.insert_at_start(70) new_linked_list.traverse_list() print("After deleting the
first node") new_linked_list.delete_at_start() new_linked_list.traverse_list() print("After
deleting the last node") new_linked_list.delete_at_end() new_linked_list.traverse_list()
print("After deleting the element by value") new_linked_list.delete_element_by_value(65)
new_linked_list.traverse_list()

## Sample Output
<img width="757" height="449" alt="image" src="https://github.com/user-attachments/assets/7b8f4501-bd81-4ddf-a69e-6711c96d8f6a" />

## Result
Thus the program was executed successfully
