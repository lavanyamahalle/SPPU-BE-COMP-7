Alright! Let’s break down **MapReduce** clearly and prepare a full 9-mark answer for your exam with points, example, and diagram. I’ll also give a memory-friendly way to recall it.

---

## **Q7(a) – MapReduce [9 Marks]**

### **1. Definition (2 Marks)**

* **MapReduce** is a **programming model** used to process **large datasets** in a **distributed computing environment**.
* It simplifies processing by dividing the task into **two main steps**: **Map** and **Reduce**.
* Popularly used in **Hadoop**, **Spark**, and big data systems.

---

### **2. Components of MapReduce (2 Marks)**

| Component          | Function                                                                   |
| ------------------ | -------------------------------------------------------------------------- |
| **Map**            | Processes input data and converts it into a **key-value pair** format.     |
| **Shuffle & Sort** | Groups all values by their **key** and sends them to the reducer.          |
| **Reduce**         | Aggregates or summarizes the grouped data to produce the **final output**. |

---

### **3. Working of MapReduce (3 Marks)**

1. **Input** – Large data is stored in a distributed file system (like HDFS).
2. **Map Function** – Each data chunk is processed independently to create **intermediate key-value pairs**.
3. **Shuffle & Sort** – System automatically groups all similar keys together and sorts them.
4. **Reduce Function** – Reducer takes each key and list of values to produce **summarized output**.
5. **Output** – Final result is written back to the file system.

---

### **4. Example (2 Marks)**

**Problem:** Count the number of times each word occurs in a large document.

* **Input:** “cat dog cat dog cat”
* **Map Output:**

  ```
  (cat,1), (dog,1), (cat,1), (dog,1), (cat,1)
  ```
* **Shuffle & Sort:**

  ```
  (cat, [1,1,1]), (dog, [1,1])
  ```
* **Reduce Output:**

  ```
  (cat, 3), (dog, 2)
  ```

---

### **5. Diagram (Optional 1 Mark)**

```
Input Data
   │
   ▼
  Map Phase  ---> (key, value)
   │
   ▼
Shuffle & Sort
   │
   ▼
  Reduce Phase ---> Final Output
```

---

### **6. Advantages (Optional extra)**

* Handles **very large datasets** efficiently.
* Works on **distributed systems**; scalable.
* Fault-tolerant: if a node fails, tasks are reassigned automatically.

---

✅ **Memory Trick:** Think **“M-S-R” → Map, Shuffle, Reduce**

* Map = Break
* Shuffle = Group
* Reduce = Combine

---

If you want, I can also **make a super neat 9-mark answer in one paragraph** that you can write directly in the exam to **score full marks**.

Do you want me to do that?

Perfect! Let’s make each note **more detailed for 6 marks**, including **definition, working, components, examples, and purpose**, so it’s exam-ready.

---

## **i) Evaluation of Web Search [6 Marks]**

* **Definition:** Evaluation of web search is the process of **measuring how effectively a search engine retrieves relevant and useful results** for a user query.
* **Importance:** Helps improve **search quality, ranking algorithms, and user satisfaction**.
* **Key Metrics:**

  1. **Precision:** Fraction of retrieved documents that are relevant.
     [
     Precision = \frac{\text{Relevant documents retrieved}}{\text{Total documents retrieved}}
     ]
  2. **Recall:** Fraction of relevant documents that are actually retrieved.
     [
     Recall = \frac{\text{Relevant documents retrieved}}{\text{Total relevant documents}}
     ]
  3. **F1-Score:** Harmonic mean of precision and recall; balances relevance and completeness.
* **Other Measures:** Mean Average Precision (MAP), Discounted Cumulative Gain (DCG) for ranking relevance.
* **Example:** Checking Google search results for a query and comparing retrieved links with a set of known relevant links.

---

## **ii) Web Crawlers and Components [6 Marks]**

* **Definition:** A web crawler (also called a spider or bot) is an automated program that **browses the web systematically** to collect web pages for indexing and search engines.
* **Purpose:** To **collect data** from websites, maintain updated indexes, and enable efficient search.
* **Working:**

  1. **Start with seed URLs** (initial web pages).
  2. **Download page content** using HTTP requests.
  3. **Extract links** and add them to the queue.
  4. **Repeat** for new URLs to cover the web.
* **Components:**

  1. **URL Frontier:** Queue of URLs waiting to be crawled.
  2. **Downloader:** Retrieves web pages from servers.
  3. **Parser:** Extracts content, links, and metadata from HTML/XML.
  4. **Indexer:** Stores processed data for search engines.
* **Example:** Googlebot, Bingbot.

---

## **iii) Web Crawler Libraries [6 Marks]**

* **Definition:** Web crawler libraries are **software frameworks** or tools that simplify building web crawlers and scraping data.
* **Purpose:** Reduce coding effort, handle HTTP requests, parsing, and data storage efficiently.
* **Popular Libraries/Tools:**

  1. **Scrapy (Python):** Powerful framework for large-scale scraping, supports asynchronous crawling.
  2. **BeautifulSoup (Python):** Parses HTML/XML to extract content; easy to use for small projects.
  3. **Selenium:** Automates browser interaction; used for **dynamic web pages** with JavaScript content.
  4. **Requests (Python):** Fetches web pages via HTTP protocol; often used with BeautifulSoup.
* **Example:** Scrapy can crawl an e-commerce site and collect product details like price, name, and rating automatically.

---

## **iv) Dynamic Ranking [6 Marks]**

* **Definition:** Dynamic ranking is the process of **ordering search results** based on changing factors like user behavior, query context, or content freshness.
* **Purpose:** Provides **personalized and relevant results** in real-time.
* **Factors Considered:**

  1. User location and preferences
  2. Click-through rates and past behavior
  3. Freshness of content
  4. Popularity of pages (e.g., PageRank)
* **Example:** Google adjusts search results for the same query based on the user’s location and recent search trends.

---

## **) The Structure of the Web [6 Marks]**

* **Definition:** The web is a **massive collection of interconnected web pages**, forming a network for users to access information.
* **Components:**

  1. **Web Pages:** HTML documents containing text, images, videos, links.
  2. **Hyperlinks:** Connect pages and create a navigable web graph.
  3. **Web Servers:** Store and deliver web content.
  4. **Clients/Browsers:** Access and render pages for users.
* **Working:** Users request pages via browser → server responds → pages are rendered → links allow navigation.
* **Example:** Wikipedia pages linked together via hyperlinks.

---

## **ii) Python Scrapy [6 Marks]**

* **Definition:** Scrapy is an **open-source Python framework** for building web crawlers and scraping data efficiently.
* **Purpose:** Automates **data extraction** from websites and supports large-scale crawling.
* **Features:**

  1. Supports **asynchronous requests** for faster crawling.
  2. Provides **spiders** to define crawling logic for websites.
  3. Built-in support for **exporting scraped data** to CSV, JSON, or databases.
  4. Handles **link extraction, data cleaning, and pagination** automatically.
* **Example:** Crawling an e-commerce site to collect product details like names, prices, and ratings.
* **Advantages:** Fast, scalable, handles large data, easy integration with pipelines for storing data.

---

If you want, I can **make a single-page diagram + key points sheet** for all 8 topics that’s **perfect for writing in 6-mark answers quickly in exams**.

Do you want me to do that?




Perfect! I’ll create **a single diagram covering all the topics** in a simple, **exam-friendly way** so you can **label and explain in 6-mark answers**. Here’s a clear textual version you can draw in exams:

---

# **Diagram for Web Search, Crawlers, and Scrapy**

```
                     ┌────────────────────┐
                     │   User Query/Input │
                     └────────┬───────────┘
                              │
                              ▼
                     ┌────────────────────┐
                     │  Web Search Engine │
                     └────────┬───────────┘
                              │
              ┌───────────────┴───────────────┐
              │                               │
              ▼                               ▼
        ┌────────────┐                  ┌─────────────┐
        │ Evaluation │                  │ Dynamic     │
        │ Metrics    │                  │ Ranking     │
        │ Precision  │                  │ (User,     │
        │ Recall     │                  │ Freshness) │
        │ F1-Score   │                  └─────────────┘
        └────────────┘
                              │
                              ▼
                     ┌────────────────────┐
                     │   Web Crawlers      │
                     └────────┬───────────┘
                              │
          ┌───────────────┬───────────────┬─────────────┐
          ▼               ▼               ▼             ▼
    ┌──────────┐    ┌──────────┐    ┌──────────┐  ┌──────────┐
    │URL       │    │Downloader│    │Parser    │  │Indexer   │
    │Frontier  │    │          │    │          │  │          │
    └──────────┘    └──────────┘    └──────────┘  └──────────┘
          │
          ▼
 ┌─────────────────────┐
 │  Web Crawler        │
 │  Libraries/Tools    │
 │  Scrapy, BS4,       │
 │  Selenium, Requests │
 └─────────────────────┘
          │
          ▼
 ┌─────────────────────┐
 │ Python Scrapy       │
 │ - Asynchronous      │
 │ - Spiders           │
 │ - Data Export       │
 │ - Pipelines         │
 └─────────────────────┘
```

---

### **How to explain in exam (6 marks)**

1. Start from **User Query/Input → Search Engine**.
2. Explain **Evaluation Metrics** (Precision, Recall, F1).
3. Explain **Dynamic Ranking** (personalization, freshness).
4. Describe **Web Crawler Components** (URL frontier, downloader, parser, indexer).
5. Mention **Libraries** (Scrapy, BS4, Selenium, Requests).
6. Highlight **Python Scrapy features** (asynchronous crawling, spiders, pipelines).

---

If you want, I can **convert this into a neat labeled diagram you can draw in under 1 min in exam**, with **colors and arrows**, perfect for full marks.

Do you want me to do that?
