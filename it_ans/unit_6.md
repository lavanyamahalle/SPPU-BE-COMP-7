Perfect! 👍
Here’s **UNIT 6 – Web & Distributed Information Retrieval (FULL, DETAILED, 9-MARK EXAM READY ANSWERS)**. This covers **Parallel Query Processing, MapReduce, Web Crawlers, Ranking, Evaluation** in full depth with **definitions, theory, examples, advantages, diagrams explanation style**.

---

# ✅ **UNIT 6 – Web & Distributed IR (Detailed Theory)**

---

## 🔹 **Q7 (a) – Describe MapReduce with suitable examples [9 Marks]**

---

### **Definition (1 Mark)**

**MapReduce** is a **programming model for processing large datasets in parallel across distributed systems**. Developed by Google, it simplifies data processing by splitting tasks into **map and reduce phases**.

---

### **Working (4 Marks)**

1. **Map Phase:**

   * Input dataset split into chunks
   * **Map function** processes each chunk and emits **key-value pairs**
   * Example: Counting word frequency → emits `(word, 1)`

2. **Shuffle & Sort Phase:**

   * Key-value pairs from all mappers are grouped by **key**
   * Ensures all values for the same key are sent to the same reducer

3. **Reduce Phase:**

   * **Reducer function** aggregates values for each key
   * Example: Sum all `1`s for each word → `(word, total_count)`

---

### **Example (2 Marks)**

* **Word Count in Web Documents:**

  * Map: Extract words from pages → `(word, 1)`
  * Reduce: Sum occurrences → `(word, total_count)`
* **Search Engine Application:**

  * Map: Parse documents, extract links or terms
  * Reduce: Aggregate link counts, build inverted index

---

### **Advantages (1½ Marks)**

* Handles **massive datasets efficiently**
* Fault-tolerant (failed tasks rerun automatically)
* Scales horizontally (add more nodes)

---

### **Conclusion (½ Mark)**

MapReduce simplifies **distributed data processing** for web-scale IR applications like **indexing, ranking, and analytics**.

---

## 🔹 **Q7 (b) – Write short note on Structure of the Web and Python Scrapy [6 Marks]**

---

### **1️⃣ Structure of the Web** – 3 Marks

**Definition:**
The web is a **large graph of interlinked documents and resources**.

**Components:**

1. **Pages** – Nodes containing information (HTML, text)
2. **Hyperlinks** – Directed edges connecting pages
3. **Web Graph** – Represents pages and links

**Example:**

* Page A links to Page B and C → edges from A to B/C

**Importance in IR:**

* Enables **link analysis** (PageRank, HITS)
* Helps web crawlers navigate the web efficiently

---

### **2️⃣ Python Scrapy** – 3 Marks

**Definition:**
Scrapy is a **Python framework for web crawling and scraping**.

**Key Features:**

* Crawl web pages and extract data
* Supports asynchronous requests for efficiency
* Handles pagination, login, and APIs

**Example:**

* Scrapy spider crawls news websites and extracts headlines, dates, and URLs

**Advantages:**

* Fast and scalable
* Easy integration with databases

---

## 🔹 **Q7 (c) – Describe Web Crawler with its components [5 Marks]**

---

### **Definition:**

A **web crawler** automatically downloads web pages and follows links to build datasets or indexes.

---

### **Components:**

1. **URL Frontier:**

   * Stores URLs to be crawled
   * Prioritizes based on policy (breadth-first, depth-first, priority)

2. **Fetcher/Downloader:**

   * Retrieves web pages over HTTP/HTTPS

3. **Parser/Analyzer:**

   * Extracts links and content
   * Converts HTML to structured data

4. **Indexer/Storage:**

   * Saves content in database or index
   * Builds inverted index for IR systems

5. **Duplicate Detection & Politeness:**

   * Avoids crawling same page multiple times
   * Respects robots.txt and rate limits

---

### **Example:**

* Googlebot crawls billions of web pages daily
* Extracts links → adds to frontier → indexes content for search

---

## 🔹 **Q8 (a) – Parallel Query Processing with examples [9 Marks]**

---

### **Definition (1 Mark)**

**Parallel Query Processing (PQP)** splits a query into **subtasks** executed simultaneously across multiple processors or servers.

---

### **Why Needed? (1 Mark)**

* Web-scale datasets → single server slow
* Reduces **query latency**
* Improves **throughput**

---

### **Working (4 Marks)**

1. **Query Decomposition:** Split query into subqueries
2. **Data Partitioning:** Split data across nodes (horizontal or vertical)
3. **Parallel Execution:** Each node executes subquery
4. **Result Merging:** Partial results combined → final answer

**Example:**

* Search engine query “Python tutorials”

  * Node 1 searches documents A–M
  * Node 2 searches documents N–Z
  * Combine results and rank

---

### **Advantages (2 Marks)**

* Faster query responses
* Handles large datasets efficiently
* Scalable with more nodes

---

### **Conclusion (1 Mark)**

PQP is critical for **web search engines and distributed IR systems** to maintain low-latency, high-throughput performance.

---

## 🔹 **Q8 (b) – Static & Dynamic Ranking [6 Marks]**

---

### **1️⃣ Static Ranking** – 3 Marks

**Definition:**
Ranking based on **precomputed metrics**, independent of query context.

**Examples:**

* **PageRank** – Link structure-based score
* **HITS** – Hub and Authority scores

**Advantages:**

* Precomputed → fast retrieval
* Good for common queries

**Limitations:**

* Ignores user query and personalization

---

### **2️⃣ Dynamic Ranking** – 3 Marks

**Definition:**
Ranking computed **at query time**, considering user query, history, and context.

**Examples:**

* TF-IDF / BM25 scoring
* Personalization based on user profile

**Advantages:**

* Query-specific relevance
* Supports personalization

**Limitations:**

* Computationally expensive

---

## 🔹 **Q8 (c) – Evaluation of Web Search [5–6 Marks]**

---

**Definition:**
Evaluates **effectiveness and efficiency** of search engines.

**Metrics:**

* Precision, Recall, MAP, NDCG
* Query latency, throughput

**Methods:**

* User studies (click-through data)
* Standard datasets (TREC, ClueWeb)

---

## 🔹 **Q8 (d) – Web Crawlers & Libraries [5 Marks]**

---

### **Libraries & Tools:**

1. **Scrapy (Python)** – Crawling, scraping, data export
2. **BeautifulSoup (Python)** – HTML parsing
3. **Apache Nutch (Java)** – Distributed web crawling

**Dynamic Crawling:**

* Handles AJAX, dynamically generated pages
* Requires headless browsers (Selenium, Puppeteer)

---

## ✅ **UNIT 6 COMPLETE – DETAILED THEORY READY (ALL Q7/Q8)**

**Notes for Exams:**

* MapReduce + Parallel Query Processing = High probability questions
* Include small diagram for **MapReduce workflow, Web Crawler components, PQP flow**
* Always mention **examples & advantages** for 9 marks

---

If you want, I can **combine ALL UNITS 3–6 into ONE single exam-ready 20–25 page memory sheet** with **diagrams, formulas, and 9-mark points for each question**, perfect for **last-minute revision**.

Do you want me to do that?
