In Tree Data Structure, traversal refers to visiting all the nodes in some specific order. 
There are three common ways to traverse a tree:

**In-Order**
**Pre-Order**
**Post-Order**. 

Let’s look at each of them:

---

### **1. In-Order Traversal (LNR)**

- **Definition:** In in-order traversal, the nodes are visited in the following order: 
  - **Left subtree**, **Node**, **Right subtree**.
  
- **Process:**
  1. Traverse the left subtree.
  2. Visit the current node.
  3. Traverse the right subtree.

- **Pseudocode:**
    ```plaintext
    Procedure InOrder(node):
        if node is NULL:
            return
        
        // Traverse left subtree
        InOrder(node.left)
        
        // Visit current node
        Print(node.value)
        
        // Traverse right subtree
        InOrder(node.right)
    ```

- **Example:**
  For the following tree:

  ```
       A
      / \
     B   C
    / \
   D   E
  ```

  The **In-Order traversal** will be: `D, B, E, A, C`.

---

### **2. Pre-Order Traversal (NLR)**

- **Definition:** In pre-order traversal, the nodes are visited in the following order: 
  - **Node**, **Left subtree**, **Right subtree**.

- **Process:**
  1. Visit the current node.
  2. Traverse the left subtree.
  3. Traverse the right subtree.

- **Pseudocode:**
    ```plaintext
    Procedure PreOrder(node):
        if node is NULL:
            return
        
        // Visit current node
        Print(node.value)
        
        // Traverse left subtree
        PreOrder(node.left)
        
        // Traverse right subtree
        PreOrder(node.right)
    ```

- **Example:**
  For the following tree:

  ```
       A
      / \
     B   C
    / \
   D   E
  ```

  The **Pre-Order traversal** will be: `A, B, D, E, C`.

---

### **3. Post-Order Traversal (LRN)**

- **Definition:** In post-order traversal, the nodes are visited in the following order: 
  - **Left subtree**, **Right subtree**, **Node**.

- **Process:**
  1. Traverse the left subtree.
  2. Traverse the right subtree.
  3. Visit the current node.

- **Pseudocode:**
    ```plaintext
    Procedure PostOrder(node):
        if node is NULL:
            return
        
        // Traverse left subtree
        PostOrder(node.left)
        
        // Traverse right subtree
        PostOrder(node.right)
        
        // Visit current node
        Print(node.value)
    ```

- **Example:**
  For the following tree:

  ```
       A
      / \
     B   C
    / \
   D   E
  ```

  The **Post-Order traversal** will be: `D, E, B, C, A`.

---

### Summary:

- **In-Order (LNR):** Left, Node, Right
- **Pre-Order (NLR):** Node, Left, Right
- **Post-Order (LRN):** Left, Right, Node
