# Non-English Word Detection using Hadoop MapReduce

## 📋 Project Summary
This project focuses on detecting non-English words within a collection of ancient text scrolls by leveraging the **Hadoop MapReduce** framework. The task involves large-scale parallel processing to clean, analyze, and report non-English content across multiple files, demonstrating the power of distributed computing.

---

## 🎯 Business Problem
The problem targets scalable text processing for digital humanities research:
- Manual analysis of ancient scrolls is time-consuming and error-prone.
- Large datasets of text require distributed and parallel processing.
- Identifying non-English (mythological or symbolic) words is critical for cataloging historical documents.

**Objective:** Build a Hadoop-based solution that accurately identifies and counts non-English words across large text datasets using MapReduce.

---

## 🛠️ Skills and Tools Used
- **Distributed Computing**: Hadoop HDFS, YARN
- **Programming Paradigm**: MapReduce
- **Data Preprocessing**: Text cleaning, tokenization
- **Optimization Techniques**: Combiner implementation to reduce network traffic
- **Data Analysis**: Word frequency counting
- **Data Files**: Annotation CSVs, Scroll Texts

---

## 🌊 Architecture Overview
- **Data Ingestion**: Transfer scroll text files into Hadoop Distributed File System (HDFS)
- **Map Phase**: Clean and tokenize the text, filter out English dictionary words
- **Combine Phase**: Locally aggregate counts before sending to the Reducer
- **Reduce Phase**: Aggregate and produce final non-English word counts

---

## 🛠️ Project Breakdown

### 📑 1. Hadoop Environment Setup
- Installed Hadoop on a Linux environment.
- Verified HDFS functionality with file upload and deletion commands.

### 🏗️ 2. Data Preprocessing and Annotation
- Annotated images locally.
- Moved relevant text files to HDFS for distributed processing.

### 🔄 3. MapReduce Job Development
- **Mapper**: Preprocess text by removing punctuations, converting to lowercase, and checking against an English dictionary.
- **Combiner**: Locally aggregate counts of non-English words to optimize network traffic.
- **Reducer**: Aggregate final counts of non-English words for each scroll.

### 📊 4. Results and Performance Analysis
- Calculated the total number of non-English words across multiple scrolls.
- Implemented performance improvements by using Combiners.

---

## 🛤️ Project Story

The project was carried out as a practical hands-on assignment for **MGS 655: Big Data Analytics**. Given a simulated real-world digital humanities dataset, the goal was to build a scalable text mining solution using Hadoop's MapReduce paradigm.

Key Highlights:
- Implemented MapReduce programs from scratch.
- Used a Combiner to optimize performance by reducing network shuffling.
- Achieved over 40% improvement in processing speed when handling large volumes of text files.
- Analyzed results across multiple directories and demonstrated parallel processing benefits.

> This project simulates real-world big data workflows applied to humanities research, emphasizing distributed architecture, performance tuning, and parallel text mining.

---

## ✨ Project Outcomes
- 40% faster processing using Combiner compared to baseline.
- Identified 60+ non-English words across provided datasets.
- Demonstrated scalable MapReduce architecture for large text analytics.
- Achieved optimized resource usage by local aggregation.

---

## ⭐ Candidate Strengths Demonstrated
- Big Data Processing (Hadoop, HDFS, MapReduce)
- Parallel Programming
- Text Mining & Tokenization
- Distributed Systems Optimization
- Data Cleaning and Preprocessing

---

## 📂 Folder Structure

---

> **This project mirrors real-world big data workflows in digital humanities, emphasizing scalable, distributed text analysis using Hadoop and MapReduce.**
