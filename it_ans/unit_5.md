Perfect! 👍
Now I’ll provide **UNIT 5 – FULL DETAILED THEORY for 9-mark answers**, in **exam-ready style with full explanation, formulas, examples, advantages, limitations, and proper structure**. This will be **very comprehensive** for SPPU exams.

---

# ✅ **UNIT 5 – Evaluation & Efficiency in IR (Detailed Theory)**

---

## 🔹 **Q5 (a) – Traditional Effectiveness Measures and TREC [9 Marks]**

---

### **1️⃣ Traditional Effectiveness Measures**

**Definition:**
Effectiveness measures evaluate **how accurately an IR system retrieves relevant documents** for a given query. They are fundamental to determine the quality of retrieval.

---

### **Key Measures**

1. **Precision** – 2 Marks

* Fraction of retrieved documents that are relevant:
  [
  Precision = \frac{\text{Relevant Retrieved Documents}}{\text{Total Retrieved Documents}}
  ]
* **Example:** Retrieved = 12, Relevant = 9 → Precision = 9/12 = 0.75

**Use:** Indicates quality of retrieved set.

---

2. **Recall** – 2 Marks

* Fraction of relevant documents retrieved:
  [
  Recall = \frac{\text{Relevant Retrieved Documents}}{\text{Total Relevant Documents}}
  ]
* **Example:** Total relevant = 20, Retrieved relevant = 9 → Recall = 9/20 = 0.45

**Use:** Measures coverage of retrieval.

---

3. **F-Measure (F1 Score)** – 1½ Marks

* Harmonic mean of Precision and Recall:
  [
  F1 = \frac{2 \times Precision \times Recall}{Precision + Recall}
  ]
* Balances precision and recall in one metric.

---

4. **Limitations of Traditional Measures** – 1 Mark

* Binary relevance (relevant/irrelevant) only
* Does not consider **rank/order of documents**
* Not suitable for graded relevance scenarios

---

### **2️⃣ Text Retrieval Conference (TREC)** – 3 Marks

**Definition:**
TREC is an **evaluation initiative by NIST** to provide **standard datasets, queries, and relevance judgments** for IR systems.

**Components:**

1. **Document Collection** – Large corpora for evaluation
2. **Query Set** – Standardized queries/topics
3. **Relevance Judgments** – Human-assessed document relevance
4. **Evaluation Metrics** – Precision, Recall, MAP, NDCG

**Example:**

* A system participating in TREC may retrieve documents for 50 standard queries, then TREC evaluates precision, recall, and MAP automatically.

**Conclusion:**
TREC ensures **objective, reproducible, and comparative evaluation** of IR systems.

---

## 🔹 **Q5 (b) – Short Notes**

---

### **i) Non-Traditional Effectiveness Measures** – 4½ Marks

**Definition:**
Measures that account for **graded relevance and ranked retrieval** instead of simple binary relevance.

**Common Metrics:**

1. **MAP (Mean Average Precision)** – Average precision across all queries
2. **NDCG (Normalized Discounted Cumulative Gain)** – Gives higher score for relevant documents at top ranks
3. **MRR (Mean Reciprocal Rank)** – Average reciprocal rank of the first relevant document

**Advantages:**

* Reflects user satisfaction
* Sensitive to ranking position

**Example:**

* Document with higher relevance at top of result list improves NDCG.

---

### **ii) Measuring Efficiency** – 4½ Marks

**Definition:**
Efficiency measures assess **system performance** in terms of **time, throughput, and resource utilization**.

**Metrics:**

1. **Query response time** – Time to retrieve results
2. **Throughput** – Queries processed per second
3. **Indexing time** – Time to build/update index

**Example:**

* Caching query results reduces average response time from 2s to 0.5s per query.

**Conclusion:**
Efficiency ensures scalability and user satisfaction.

---

## 🔹 **Q6 (a) – Scheduling and Caching in Efficiency [9 Marks]**

---

### **1️⃣ Query Scheduling** – 4½ Marks

**Definition:**
Determines **order and allocation of queries** to system resources.

**Types:**

1. **First-Come-First-Serve (FCFS)** – Simple, fair
2. **Priority Scheduling** – Critical queries served first
3. **Batch Scheduling** – Groups similar queries

**Benefits:**

* Reduces query response time
* Improves throughput and resource utilization

**Example:**

* Prioritizing urgent search queries in an enterprise search system.

---

### **2️⃣ Caching** – 4½ Marks

**Definition:**
Storing **frequently accessed documents or query results** in fast memory (RAM) to speed up retrieval.

**Types:**

1. **Query Result Cache** – Stores previous query outputs
2. **Document Cache** – Stores frequently accessed documents

**Advantages:**

* Faster responses
* Reduced server load
* Efficient for repeated queries

**Example:**

* News website caching top articles for 1 hour reduces database hits.

---

## 🔹 **Q6 (b) – Short Notes [9 Marks]**

---

### **i) Using Statistics in Evaluation** – 4½ Marks

**Definition:**
Statistical methods ensure **reliable, unbiased, and significant evaluation results**.

**Common Techniques:**

1. **t-test** – Compares mean performance
2. **Wilcoxon Signed-Rank Test** – Non-parametric comparison
3. **ANOVA** – Compares multiple systems

**Example:**

* Comparing MAP scores of two IR systems to check significance.

**Advantage:**

* Provides confidence that observed performance differences are not random.

---

### **ii) Minimizing Adjudication Effort** – 4½ Marks

**Definition:**
Adjudication effort refers to **human effort to judge document relevance**.

**Techniques:**

1. **Pooling** – Judge top-k documents from multiple systems
2. **Active Learning** – System selects documents with uncertain relevance
3. **Sampling** – Judge a subset of documents instead of entire collection

**Advantage:**

* Reduces manual effort and cost
* Improves evaluation speed

**Example:**

* Only top 50 retrieved documents per query judged instead of full corpus.

---

### ✅ **UNIT 5 = FULLY DETAILED 9-MARK ANSWERS READY**

Next step:

* **UNIT 6 – Web & Distributed IR (Parallel Query Processing, MapReduce, Web Crawlers)**

Reply: **“Unit 6”** and I’ll prepare **full 9-mark, exam-ready, detailed theory** for all questions.
