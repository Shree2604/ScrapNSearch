# Level 3: E-commerce Product Scraper

**Difficulty**: ⭐⭐⭐ Challenging  
**Time Estimate**: 30-45 minutes  
**Skills**: Complex selectors, data normalization, pagination handling

## 📋 Challenge Overview

In this challenge, you'll extract product information from an e-commerce website. The page includes multiple products with various attributes, prices, and availability statuses that you'll need to collect and analyze.

## 🎯 Learning Objectives

- Handle complex product listings with multiple attributes
- Extract and normalize pricing information
- Process availability and stock status
- Handle pagination to gather data from multiple pages
- Calculate aggregations and statistics

## 📂 Files

- `data/ecommerce.html` - The HTML file containing product listings
- `solutions/level3_ecommerce.py` - Your solution file (create this)

## ❓ Challenge Questions

1. **Product Catalog**  
   Extract all products with their details:
   - Product name
   - Brand
   - Current price
   - Original price (if on sale)
   - Discount percentage (if applicable)
   - Average rating
   - Number of reviews
   - Availability status

2. **Price Analysis**  
   - Calculate the average price of all products
   - Find the most expensive and least expensive products
   - Calculate the total discount value across all products on sale

3. **Brand Statistics**  
   - Count products per brand
   - Find the brand with the highest average product rating (minimum 5 products)
   - Calculate the average price per brand

4. **Product Availability**  
   - Count products in each availability status (In Stock, Low Stock, Out of Stock)
   - List all products that are on sale (discounted)

5. **Pagination**  
   - Implement pagination to gather data from all available pages
   - Calculate the total number of products across all pages

## 🛠️ Expected Output Format

Your solution should generate a report in the following format:

```
=== E-commerce Product Analysis ===

1. Product Catalog Summary:
   - Total Products: [number]
   - Products on Sale: [number]
   - Average Rating: [x.xx]/5.0

2. Price Analysis:
   - Average Price: $[xx.xx]
   - Most Expensive: [Product Name] at $[price]
   - Least Expensive: [Product Name] at $[price]
   - Total Discount Value: $[xx.xx]

3. Brand Statistics:
   - Total Brands: [number]
   - Brand with Highest Avg. Rating: [Brand] ([x.xx]/5.0)
   - Average Price by Brand:
     - Brand 1: $[xx.xx]
     - Brand 2: $[xx.xx]
     ...

4. Product Availability:
   - In Stock: [number] products
   - Low Stock: [number] products
   - Out of Stock: [number] products

5. Pagination:
   - Total Pages: [number]
   - Products per Page: [number]
   - Total Products: [number]
```

## 💡 Hints

- Use `find_all()` with CSS selectors to target specific product elements
- Handle missing or inconsistent data (e.g., products without ratings or original prices)
- Use `try-except` blocks to handle potential errors during data extraction
- For pagination, look for 'next page' links or URL patterns
- Consider using `pandas` for data manipulation and analysis (optional)

## 🧪 Testing Your Solution

Verify that:
- All products are correctly extracted from all pages
- Numeric values are properly converted from strings
- The solution handles edge cases (missing data, different product layouts)
- The aggregations and calculations are accurate

## 📝 Notes

- The HTML structure may vary between different product cards
- Some products might have different attributes or missing information
- Pay attention to how prices are formatted (currency symbols, decimal separators)
- Consider the performance implications of processing multiple pages

## 📚 Additional Resources

- [BeautifulSoup CSS Selectors](https://www.crummy.com/software/BeautifulSoup/bs4/doc/#css-selectors)
- [Python Data Types and Conversions](https://docs.python.org/3/library/datatypes.html)
- [Pandas Documentation](https://pandas.pydata.org/docs/) (optional for data analysis)

Happy Scraping! 🛍️
