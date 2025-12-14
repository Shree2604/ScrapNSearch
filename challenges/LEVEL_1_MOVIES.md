# Level 1: Movie Database Scraper

**Difficulty**: ⭐ Easy  
**Time Estimate**: 15-20 minutes  
**Skills**: Basic tag finding, attribute extraction, data aggregation

## 📋 Challenge Overview

In this challenge, you'll extract information about movies from the provided HTML file. You'll need to parse the movie data and answer specific questions about the movie collection.

## 🎯 Learning Objectives

- Practice basic HTML parsing with BeautifulSoup
- Extract text content and attributes from HTML elements
- Perform basic data aggregation and analysis
- Work with different types of HTML elements and their attributes

## 📂 Files

- `data/movies.html` - The HTML file containing movie data
- `solutions/level1_movies.py` - Your solution file (create this)

## ❓ Challenge Questions

1. **Highest Rated Movies**  
   Which movie(s) have the highest rating? (Return all if there's a tie)

2. **Recent Releases**  
   How many movies were released after 2020?

3. **Top Rated Movies**  
   List all movie titles with a rating above 8.5

4. **Popular Genres**  
   What is the most common genre across all movies?

5. **Prolific Directors**  
   Which director has the most movies in this list?

## 🛠️ Expected Output Format

Your solution should print the answers in the following format:

```
1. Highest Rated Movie(s): [List of movie names]
2. Movies released after 2020: [Number]
3. Movies with rating > 8.5: [List of movie names]
4. Most common genre: [Genre name]
5. Director with most movies: [Director name]
```

## 💡 Hints

- Use `find_all()` to locate all movie elements
- Extract text using `.text` and attributes using dictionary notation `['attribute']`
- For the highest rating, you might want to first find the maximum rating value
- For counting movies after 2020, check the release year in the movie details
- Use a dictionary to count genres and director appearances

## 🧪 Testing Your Solution

Run your script and verify the output matches the expected format. Check that:
- All movie titles are correctly extracted
- The rating comparisons are accurate
- The counts and aggregations are correct

## 📝 Notes

- Pay attention to the HTML structure and class names
- Handle potential missing data gracefully
- Your solution should work for any similar HTML structure, not just the provided example

## 📚 Additional Resources

- [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Python String Methods](https://docs.python.org/3/library/stdtypes.html#string-methods)
- [Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)

Happy Scraping! 🎬
