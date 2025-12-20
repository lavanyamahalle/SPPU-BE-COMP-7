Understood 👍
I’ll give you **FULL, EXAM-READY 9-MARK ANSWERS**, **one question at a time**, written in **SPPU scoring format** (definition → diagram → points → example → conclusion).

⚠️ Important (to keep quality high):
If I dump **all units together**, it will be **too long to revise**.
So I’ll give answers **UNIT-WISE**, exactly matching **DEC 2025 predicted questions**.

I’ll start with **UNIT 3 (Q1 & Q2)** now.
After that, you just say **“Next Unit”**.

---

# ✅ UNIT 3 – Data Compression & Index Maintenance

## **Q1 (9 Marks)**

### **Explain Data Compression with Huffman Coding.**

---

### **Definition (1 mark)**

**Data Compression** is the process of reducing the size of data so that it requires less storage space and less transmission time. Huffman Coding is a **lossless compression technique** used widely in Information Retrieval systems.

---

### **Why Compression is needed in IR (1 mark)**

* Large document collections
* Faster disk access
* Reduced storage cost
* Efficient inverted index storage

---

### **Huffman Coding – Concept (2 marks)**

Huffman Coding assigns:

* **Shorter codes to frequent symbols**
* **Longer codes to less frequent symbols**

It uses a **binary tree** called a **Huffman Tree**.

---

### **Steps of Huffman Coding (3 marks)**

1. Calculate frequency of each symbol
2. Create leaf nodes for each symbol
3. Insert all nodes into a priority queue (min-heap)
4. Repeatedly:

   * Remove two nodes with lowest frequency
   * Merge them into a new node
   * Insert back into queue
5. Assign:

   * Left edge → 0
   * Right edge → 1
6. Generate codes by traversing the tree

---

### **Example (2 marks)**

| Symbol | Frequency |
| ------ | --------- |
| A      | 5         |
| B      | 9         |
| C      | 12        |
| D      | 13        |
| E      | 16        |
| F      | 45        |

Final Huffman Codes:

* F → 0
* C → 100
* D → 101
* A → 1100
* B → 1101
* E → 111

👉 Frequent symbol **F** gets shortest code.

---

### **Advantages (1 mark)**

* Optimal prefix code
* No ambiguity in decoding
* Lossless compression

---

### **Conclusion (½ mark)**

Huffman Coding efficiently compresses textual data in IR systems by minimizing average code length while preserving original information.

---

---

## **Q1 (b) (9 Marks)**

### **Explain Context-Aware Compression Methods.**

---

### **Definition (1 mark)**

**Context-Aware Compression** techniques use the **surrounding context** of symbols to predict the probability of the next symbol and achieve better compression.

---

### **Why Context-Aware Compression? (1 mark)**

* Simple methods ignore symbol dependency
* Natural language has strong context patterns
* Better prediction → better compression

---

### **Working Principle (2 marks)**

* Probability of a symbol depends on **previous symbols**
* Uses conditional probabilities:

[
P(x_i | x_{i-1}, x_{i-2}, ...)
]

---

### **Types of Context-Aware Compression (4 marks)**

#### **1. PPM (Prediction by Partial Matching)**

* Uses fixed-length context
* Predicts next symbol using previous k symbols
* Higher order → better compression

#### **2. Markov Models**

* Probability depends on last symbol(s)
* Used in language modeling

#### **3. Adaptive Arithmetic Coding**

* Probabilities updated dynamically
* Combines context modeling + arithmetic coding

#### **4. n-gram Based Compression**

* Uses frequent word sequences
* Common in text compression

---

### **Advantages (1 mark)**

* Higher compression ratio
* Exploits language structure
* Effective for large text collections

---

### **Conclusion (½ mark)**

Context-aware compression significantly improves compression efficiency by utilizing symbol dependencies, making it suitable for IR systems.

---

---

## **Q2 (9 Marks)**

### **Write short notes on:**

i) Decoding Performance
ii) Document Reordering
iii) Arithmetic Coding

---

### **i) Decoding Performance (3 marks)**

* Measures **speed of decompression**
* Faster decoding improves query response time
* Important in real-time IR systems

Factors affecting decoding performance:

* Code complexity
* Memory access pattern
* CPU cache behavior

---

### **ii) Document Reordering (3 marks)**

* Documents are reordered to:

  * Improve compression
  * Reduce gap values in posting lists
* Similar documents placed closer

Benefits:

* Smaller gaps
* Better compression
* Faster query processing

---

### **iii) Arithmetic Coding (3 marks)**

* Encodes entire message into a **single fractional number**
* Uses probability ranges instead of fixed codes
* More efficient than Huffman for skewed data

Advantages:

* Near optimal compression
* Handles fractional probabilities

---

---

## **Q2 (b) (9 Marks)**

### **Explain Invalidation List, Garbage Collection, and Document Modification.**

---

### **1. Invalidation List (3 marks)**

* Used when documents are deleted
* Document IDs marked as invalid
* Avoids immediate index rebuilding

Advantage:

* Fast deletion
* Low overhead

---

### **2. Garbage Collection (3 marks)**

* Periodic cleanup process
* Removes invalid postings
* Reclaims unused space

Steps:

* Scan index
* Identify invalid docs
* Compact index

---

### **3. Document Modification (3 marks)**

* Modifying document = delete + reinsert
* Old version invalidated
* New version indexed

Challenges:

* Index consistency
* Performance overhead

---

### **Conclusion (½ mark)**

These techniques help maintain **dynamic inverted indexes** efficiently without frequent full reindexing.

---

✅ **UNIT 3 DONE (36 MARKS READY)**

Say **“Next Unit”** and I’ll give **UNIT 4 (Categorization, Probabilistic Models, Language Models)** in the **same 9-mark perfect format**.
