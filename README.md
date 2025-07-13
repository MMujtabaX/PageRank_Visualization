# 🕸️ PageRank Spider - Web Crawler & Visualizer 

This project implements a basic **web crawler**, **link extractor**, **PageRank calculator**, and **visualizer** using Python and SQLite. It is part of the **Capstone Project** from the [Python for Everybody](https://www.py4e.com/) specialization by **Dr. Charles Severance (Dr. Chuck)**.

---

## 🌐 What It Does

- Crawls a website and stores internal links (`spider.py`)
- Calculates PageRank scores over multiple iterations (`sprank.py`)
- Dumps top-ranked pages and incoming link count (`spdump.py`)
- Generates a **network graph visualization** (`spjson.py` ➜ `spider.js` ➜ `force.html`)

---


![PageRank Demo](https://media.licdn.com/dms/image/v2/D5622AQEWUMe1mUZlGQ/feedshare-shrink_800/B56ZRjfJF0GQAg-/0/1736835899940?e=2147483647&v=beta&t=AHPnv7yp5ZFW-nnn_EJCIJ_aB0zdoT0b3u2BaNUoUiM)
> Replace with a screen-recorded GIF of your `force.html` graph if available.

---

## 📁 Project Structure

| File          | Description |
|---------------|-------------|
| `spider.py`   | Crawl web pages, extract links, and populate the SQLite DB (`spider.sqlite`) |
| `sprank.py`   | Apply the **PageRank** algorithm iteratively to update `new_rank` |
| `spdump.py`   | Print top 50 ranked pages with inbound links |
| `spjson.py`   | Export graph structure as JSON (`spider.js`) to visualize in `force.html` |
| `spider.sqlite` | SQLite database storing URLs, HTML content, and PageRank scores |
| `spider.js`   | Auto-generated file with PageRank and graph nodes/edges |
| `force.html`  | Visualize `spider.js` data as an interactive force-directed graph |
| `README.md`   | Project documentation |

---

## 🛠️ How to Use

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/pagerank-spider.git
cd pagerank-spider
