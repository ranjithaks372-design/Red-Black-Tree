# Red-Black-Tree

A menu-driven implementation of a Red-Black Tree using C. The project demonstrates insertion, deletion, searching, finding minimum and maximum elements, tree rotations, and balancing operations.

## Features

- Insert a node
- Delete a specific node
- Search for a node
- Find minimum element
- Find maximum element
- Delete minimum element
- Delete maximum element
- Display the tree structure
- Display node colors
- Inorder traversal
- Input validation
- Duplicate-value handling

## Red-Black Tree Properties

The implementation maintains the following Red-Black Tree properties:

1. Every node is either Red or Black.
2. The root node is always Black.
3. NULL leaves are considered Black.
4. A Red node cannot have a Red child.
5. Every path from a node to its descendant NULL leaves contains the same number of Black nodes.

These properties help maintain a balanced tree and ensure efficient operations.

## Operations

### Insertion

A new element is inserted according to Binary Search Tree rules. The newly inserted node is initially Red. If a Red-Black Tree property is violated, the tree is balanced using recoloring and rotations.

### Deletion

A selected node can be deleted while maintaining the Binary Search Tree structure. If deletion causes a Red-Black Tree property violation, deletion fix-up operations restore the required properties.

### Rotations

The project uses:

- Left Rotation
- Right Rotation

Rotations are used to restructure the tree during insertion and deletion while preserving the Binary Search Tree ordering.

### Search

The search operation follows Binary Search Tree ordering to locate the requested element.

### Minimum and Maximum

The minimum element is obtained by traversing the leftmost path, while the maximum element is obtained by traversing the rightmost path.

## Time Complexity

| Operation | Time Complexity |
|-----------|-----------------|
| Search | O(log n) |
| Insertion | O(log n) |
| Deletion | O(log n) |
| Find Minimum | O(log n) |
| Find Maximum | O(log n) |
| Delete Minimum | O(log n) |
| Delete Maximum | O(log n) |

Space complexity: O(n)

## Project Structure

| File | Description |
|------|-------------|
| `main.c` | Main program and menu-driven interface |
| `main.h` | Structure definitions, macros, and function declarations |
| `insert.c` | Node insertion |
| `insert_fix.c` | Fixes Red-Black Tree properties after insertion |
| `delete.c` | Deletes a specific node |
| `delete_fixup.c` | Fixes Red-Black Tree properties after deletion |
| `delete_min.c` | Deletes the minimum node |
| `delete_max.c` | Deletes the maximum node |
| `find_min.c` | Finds the minimum element |
| `find_max.c` | Finds the maximum element |
| `search.c` | Searches for an element |
| `rotate.c` | Implements left and right rotations |
| `display.c` | Displays the tree structure and inorder traversal |
| `validate.c` | Handles integer input validation |
| `makefile` | Automates compilation and cleaning |

## Menu

```text
1. Insert
2. Delete
3. Find Minimum
4. Find Maximum
5. Delete Minimum
6. Delete Maximum
7. Display
8. Search
9. Exit
