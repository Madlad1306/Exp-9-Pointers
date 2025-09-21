# Pointers in C++

**AIM:**
To study and implement the concept of **pointers** in C++.

**SOFTWARE USED:**
Visual Studio Code (VS Code)

---

## THEORY

A **pointer** is a special type of variable that stores the **memory address** of another variable. In C++, pointers are powerful tools used for **direct memory access, dynamic memory allocation, efficient array/string handling, and function parameter passing**.

---

### 1. **Pointer Basics**

* Declared using an asterisk (`*`).
* Example:

  ```cpp
  int x = 10;
  int *ptr = &x; // ptr stores the address of x
  ```
* `*ptr` → dereferences the pointer (accesses value stored at the address).
* `&x` → returns the address of variable `x`.

---

### 2. **Pointer Arithmetic**

* Pointers can be incremented/decremented.
* Incrementing moves the pointer to the **next memory block of its data type**:

  * `int*` → moves by 4 bytes (on most systems).
  * `double*` → moves by 8 bytes.
  * `char*` → moves by 1 byte.

---

### 3. **Pointers and Arrays**

* The name of an array itself is a pointer to the first element.
* Example:

  ```cpp
  arr[i] ≡ *(arr + i)
  ```

---

### 4. **Strings and Pointers**

* C-style strings are arrays of characters ending with `'\0'`.
* A `char*` can traverse each character until the null terminator.

---

### 5. **Common Applications**

* Array traversal without indexing.
* Array/string reversal using two pointers.
* Summation of elements using dereferencing.
* Palindrome checking.

---

### 6. **Advantages**

* Faster access and modification.
* Enables **dynamic memory allocation**.
* Allows passing **large structures (arrays) to functions** without copying.

---

### 7. **Precautions**

* Avoid uninitialized pointers (they cause **undefined behavior**).
* Accessing invalid memory leads to **segmentation faults**.
* Always validate pointers before dereferencing.

---

## ALGORITHMS

### 1️⃣ Pointer Arithmetic on Different Data Types

**Aim:** Demonstrate how pointer increment changes addresses depending on the data type.

**Steps:**

1. Start
2. Declare variables of type `int`, `double`, `bool`.
3. Create pointers for each.
4. Print their initial addresses.
5. Increment each pointer by 1.
6. Print new addresses.
7. Stop

---

### 2️⃣ Sum of Array Elements Using Pointers

**Aim:** Calculate sum of array elements using pointer arithmetic.

**Steps:**

1. Start
2. Declare and initialize integer array.
3. Set pointer to first element.
4. Initialize `sum = 0`.
5. For each element → `sum += *(ptr + i)`.
6. Print `sum`.
7. Stop

---

### 3️⃣ Reverse an Array Using Pointers

**Aim:** Reverse an array using two pointers.

**Steps:**

1. Start
2. Declare and initialize array.
3. Set one pointer to start, another to end.
4. While start < end:

   * Swap values at both pointers.
   * Increment start, decrement end.
5. Print reversed array.
6. Stop

---

### 4️⃣ Check Palindrome String Using Pointers

**Aim:** Determine if a string is palindrome using pointers.

**Steps:**

1. Start
2. Input string.
3. Initialize two pointers → start (first char), end (last char).
4. While start < end:

   * If `*start != *end` → Not Palindrome.
   * Else → increment start, decrement end.
5. If loop completes → Palindrome.
6. Stop

---

## CONCLUSION

Pointers are among the most **powerful features of C++**, allowing **direct memory manipulation, dynamic allocation, efficient array/string operations, and optimized function calls**.
However, they must be used carefully to avoid **segmentation faults, dangling pointers, or memory leaks**. Proper understanding of pointers is crucial for mastering **low-level programming concepts** in C++.

---
