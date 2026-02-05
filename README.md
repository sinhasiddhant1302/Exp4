# 🐍 Study of Sets in Python

> **Experiment No:** 4  
> **Topic:** Understanding Sets 

## 🎯 Aim
To study set operations.

---

## 📖 Theory
Sets in Python are collections that share similarities with lists and tuples but have distinct characteristics:

* **🚫 Unordered:** The order of elements is random and can change; items are not stored in a specific sequence.
* **🔢 No Indexing:** You cannot access items using an index (e.g., `set[0]` will raise an error).
* **✨ Unique Elements:** Duplicate values are automatically removed upon creation.
* **🧮 Math-Ready:** Optimized for mathematical operations like unions, intersections, and differences.



---

## 🛠️ Function & Operation Reference

### **Creation & Basics**
| Function | Description |
| :--- | :--- |
| `set()` | Creates a new set; automatically removes duplicates from a list/tuple. |
| `frozenset()` | Creates an **immutable** set (cannot be modified after creation). |
| `print()` | Displays the output or content of the set to the console. |
| `type()` | Returns object type (e.g., `<class 'set'>` or `<class 'frozenset'>`). |

### **Modifying Sets**
| Method | Description |
| :--- | :--- |
| `.add()` | Adds a single new element to the set. |
| `.remove()` | Removes an element; **raises an error** if the element is missing. |
| `.discard()` | Removes an element; **does NOT raise an error** if the element is missing. |

### **Mathematical Operations**
| Symbol | Operation | Description |
| :---: | :--- | :--- |
| **`\|`** | **Union** | Combines sets (All unique elements from both). |
| **`&`** | **Intersection** | Elements common to both sets. |
| **`-`** | **Difference** | Elements in the first set but not the second. |
| **`^`** | **Symmetric Diff** | Elements in either set, but **not** in both. |

---

## 💻 Problem Statements & Algorithms

### 1️⃣ Unique Event Participants
> **Goal:** Extract a list of unique names from a registration list containing duplicates.

**Algorithm:**
1.  **Start.**
2.  Initialize a list `participants` with duplicate names.
3.  Convert the list to a set `unique_participants` (duplicates removed auto-magically).
4.  Display the result.
5.  **Stop.**

### 2️⃣ Common Subjects
> **Goal:** Find subjects common across three different students.

**Algorithm:**
1.  **Start.**
2.  Initialize three sets (`student1`, `student2`, `student3`).
3.  Perform **Intersection** (`&`) across all three sets.
4.  Display the common subject(s).
5.  **Stop.**

### 3️⃣ Club Membership Analysis
> **Goal:** Analyze Cricket and Football club memberships to find specific student groups.

**Algorithm:**
1.  **Start.**
2.  Initialize `set_cricket` and `set_football`.
3.  **Both Clubs:** Use Intersection (`&`).
4.  **Only Cricket:** Use Difference (`cricket - football`).
5.  **Only Football:** Use Difference (`football - cricket`).
6.  **Exclusively One Club:** Use Symmetric Difference (`^`).
7.  Display all results.
8.  **Stop.**

### 4️⃣ Absent Students
> **Goal:** Identify absent students by comparing the total class list against the present list.

**Algorithm:**
1.  **Start.**
2.  Initialize `setstd` (Total students) and `presentstd` (Present students).
3.  Calculate **Difference** (`setstd - presentstd`).
4.  Display the resulting set of absent students.
5.  **Stop.**

### 5️⃣ Remove Invalid Entries
> **Goal:** Remove a discontinued course code from a set of valid courses.

**Algorithm:**
1.  **Start.**
2.  Initialize `subject` set with course codes.
3.  Use `.discard()` to safely remove the discontinued code (e.g., "Ecsf101").
4.  Display the updated set.
5.  **Stop.**

---

## ✅ Conclusion
We successfully verified the implementation of **Sets in Python**. We explored their unique properties (unordered, distinct elements) and applied them to solve real-world data problems using mathematical operations like Union, Intersection, and Difference.
