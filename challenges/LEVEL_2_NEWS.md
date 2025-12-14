# Level 2: News Article Scraper

**Difficulty**: ⭐⭐ Medium  
**Time Estimate**: 20-30 minutes  
**Skills**: Text processing, data extraction, handling nested elements

## 📋 Challenge Overview

In this challenge, you'll extract information from a news website's HTML structure. The page contains multiple news articles with various metadata that you'll need to collect and analyze.

## 🎯 Learning Objectives

- Work with complex nested HTML structures
- Extract and clean text content
- Handle different types of article metadata
- Process and analyze extracted data

## 📂 Files

- `data/news.html` - The HTML file containing news articles
- `solutions/level2_news.py` - Your solution file (create this)

## ❓ Challenge Questions

1. **Headline Extraction**  
   Extract and list all article headlines

2. **Article Metadata**  
   For each article, extract the following:
   - Publication date
   - Author name
   - Number of comments
   - Reading time

3. **Category Analysis**  
   Count how many articles are in each category (e.g., Technology, Politics, Sports)

4. **Trending Topics**  
   Extract and count all article tags, then list the top 3 most common tags

5. **Featured Image**  
   Extract the URL of the featured image for each article

## 🛠️ Expected Output Format

Your solution should print the answers in a clear, readable format. For example:

```
1. Total Articles: [number]

2. Article Metadata:
   - Title: [title]
     Date: [date]
     Author: [author]
     Comments: [number]
     Reading Time: [time]
   - [Next article...]

3. Articles by Category:
   - Category 1: [count]
   - Category 2: [count]
   ...

4. Top 3 Tags:
   1. [tag1] - [count]
   2. [tag2] - [count]
   3. [tag3] - [count]

5. Featured Images:
   - [Article 1 Title]: [image URL]
   - [Article 2 Title]: [image URL]
   ...
```

## 💡 Hints

- Use `find_all()` with appropriate filters to locate article containers
- Pay attention to the HTML structure and class names
- Use string manipulation to clean up extracted text
- For counting categories and tags, consider using Python's `collections.Counter`
- Handle cases where certain metadata might be missing

## 🧪 Testing Your Solution

Verify that:
- All articles are processed
- The metadata is correctly extracted and formatted
- The counts and aggregations are accurate
- Your solution handles edge cases (missing data, different article formats)

## 📝 Notes

- The HTML structure may contain nested elements that require careful navigation
- Some articles might be missing certain metadata
- Pay attention to relative vs. absolute URLs for images
- Your solution should be robust enough to handle minor structural changes

## 📚 Additional Resources

- [BeautifulSoup find_all() documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/#find-all)
- [Python String Operations](https://docs.python.org/3/library/string.html)
- [Python Collections Counter](https://docs.python.org/3/library/collections.html#collections.Counter)

Happy Scraping! 📰
