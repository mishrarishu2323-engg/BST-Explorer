# Binary Search Tree Explorer

An interactive web app that visualizes how a Binary Search Tree (BST) changes as numbers are inserted, searched, deleted or updated. It also shows the Inorder, Preorder and Postorder traversals.

Developed as an **HCL GUVI Training Project**.

**Live demo:** [https://bst-explorer.onrender.com](https://bst-explorer.onrender.com)

## Features

- **Insert:** walks the path from the root, highlights every comparison, then places the new node.
- **Search:** highlights the path and shows found or not found with the number of comparisons.
- **Delete:** handles all three cases (leaf node, one child, two children).
- **Update value:** replaces an old value with a new one while keeping the BST rule intact (delete + insert).
- **Duplicate handling:** a repeated value is not inserted, the existing node turns red and a clear message is shown.
- **Traversals:** Inorder, Preorder and Postorder results are always visible, each with an animation.
- **Extras:** add random numbers, clear the tree, and see the node count and height.
- **Login system:** User Login, Create Account (Full Name, Email Address, Password) and Logout.
- **Learn more page:** explains BST operations, traversals, recursion and time complexity.
- Responsive layout.

## Tech stack

- HTML, CSS and JavaScript (no frameworks, no libraries)
- Tree drawn with SVG
- Browser storage (`localStorage` and `sessionStorage`) for the login system

## Data structures and concepts used

- Binary Search Tree
- Recursion (insert, search, delete and all three traversals)
- Tree traversals: Inorder, Preorder, Postorder

## Time complexity

| Operation | Balanced tree | Skewed tree (worst case) |
|-----------|---------------|--------------------------|
| Insert    | O(log n)      | O(n)                     |
| Search    | O(log n)      | O(n)                     |
| Delete    | O(log n)      | O(n)                     |
| Traversal | O(n)          | O(n)                     |

Here `n` is the number of nodes. Insert, search and delete take O(h) time, where `h` is the height of the tree.

## Project structure

```
.
├── index.html    # opens the login page
├── login.html    # User Login and Create Account
├── bst.html      # BST Explorer (dashboard)
├── learn.html    # Learn more page
└── README.md
```

## How to run locally

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. Open `index.html` in a browser.
   Or use the **Live Server** extension in VS Code: right-click `index.html` and choose **Open with Live Server**.

No installation or build step is needed.

## How to use

1. Create an account, then log in.
2. Type a number in **Value** and click **Insert**.
3. Use **Search** to find a value and **Delete** to remove it.
4. To change a value, enter the old value in **Value**, the new one in **New value**, and click **Update**.
5. Use the **Animate** buttons to see each traversal order on the tree.
6. Open the **Learn more** tab to read how a BST works.

Tip: insert `1, 2, 3, 4, 5` one by one to see a skewed tree and watch the height grow.

## Limitations

- The login system is a front-end demo only. Accounts are stored in the browser's `localStorage`, so they stay in that browser and are not secure. A real application needs a backend and a database.
- Duplicate values are not allowed in the tree.

## Team

**Developed as HCL GUVI Training Project**
B.Tech Computer Science & Engineering | 2nd Year

- Rishu Mishra
- Pranshu
- Ravi Ranjan Anand
- Omkar Dubey
- Rishabh Mishra