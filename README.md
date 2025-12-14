# 🕵️‍♂️ Scrape & Guess - Web Scraping Challenge Game

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)


> An interactive educational game designed to teach web scraping fundamentals through hands-on challenges using BeautifulSoup4.


## 🎯 Overview

**Scrape & Guess** is an educational web scraping game that helps students and developers learn data extraction techniques in a fun, competitive environment. Players scrape HTML files or live websites to answer progressively challenging questions.

### Learning Objectives

- Master HTML parsing with BeautifulSoup4
- Understand CSS selectors and DOM navigation
- Practice data extraction and transformation
- Learn web scraping best practices
- Develop problem-solving skills


## ✨ Features

- **Offline Mode**: Practice with static HTML files (no internet required)
- **Progressive Difficulty**: Easy → Medium → Hard → Expert challenges
- **Auto-Validation**: Automated answer checking system
- **Real-World Scenarios**: Movie databases, news sites, e-commerce layouts
- **Educational**: Includes detailed solutions and explanations
- **Extensible**: Easy to add custom challenges


## 🚀 Installation

### Prerequisites

- Python 3.8 or higher
- pip package manager
- Text editor or IDE

### Setup Instructions

```bash
# Clone the repository
git clone https://github.com/Shree2604/ScrapNSearch.git
cd ScrapNSearch

# Create virtual environment (recommended)
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

## 🎮 Quick Start

1. **Choose a challenge level** from the `challenges/` directory
2. **Read the HTML file** in the `data/` directory to understand the structure
3. **Write your scraping script** to extract data and answer questions
4. **Quote your answer** & Update .py file in your fork 

## 📊 Challenge Levels

| Level | File | Difficulty | Time | Skills Required |
|-------|------|------------|------|-----------------|
| 1 | [movies.html](data/movies.html) | ⭐ Easy | 15-20 min | Basic tag finding, attribute extraction |
| 2 | [news.html](data/news.html) | ⭐⭐ Medium | 20-30 min | Text processing, data aggregation |
| 3 | [ecommerce.html](data/ecommerce.html) | ⭐⭐⭐ Hard | 30-45 min | Complex selectors, nested data |
| 4 | [social_media.html](data/social_media.html) | ⭐⭐⭐⭐ Expert | 45-60 min | Dynamic content, edge cases |

**Detailed challenge instructions**: See individual files in the [`challenges/`](challenges/) directory.



## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
