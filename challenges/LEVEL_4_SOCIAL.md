# Level 4: Social Media Data Scraper

**Difficulty**: ⭐⭐⭐⭐ Expert  
**Time Estimate**: 45-60 minutes  
**Skills**: Dynamic content handling, complex data relationships, API simulation

## 📋 Challenge Overview

In this advanced challenge, you'll extract and analyze data from a social media feed. The page includes user posts, comments, likes, shares, and other engagement metrics that you'll need to collect and process.

## 🎯 Learning Objectives

- Handle dynamic content loading and infinite scroll
- Extract and relate nested data (posts, comments, reactions)
- Process timestamps and relative time formats
- Analyze engagement metrics and user interactions
- Handle authentication and session management

## 📂 Files

- `data/social_media.html` - The HTML file containing social media feed
- `solutions/level4_social.py` - Your solution file (create this)
- `data/credentials.json` - Contains mock authentication tokens (if needed)

## ❓ Challenge Questions

1. **User Activity**
   - Extract all posts with their metadata:
     - Username and profile link
     - Post content and timestamp
     - Number of likes, comments, and shares
     - Post type (text, image, video, etc.)

2. **Engagement Analysis**
   - Calculate average engagement rate per post
   - Identify the most engaging post (highest combined likes + comments + shares)
   - Find the most active user (most posts)
   - Calculate the average time between posts

3. **Content Analysis**
   - Extract and count all hashtags
   - Identify trending topics (most mentioned words excluding common words)
   - Categorize posts by type (text, image, video, etc.)

4. **Temporal Analysis**
   - Group posts by time of day (morning, afternoon, evening, night)
   - Calculate posting frequency over time
   - Identify peak activity hours

5. **User Interactions**
   - Extract comment threads and their structure
   - Identify most active commenters
   - Find posts with the most discussion (most comments)

## 🛠️ Expected Output Format

Your solution should generate a comprehensive report:

```
=== Social Media Analysis Report ===

1. User Activity Summary:
   - Total Posts: [number]
   - Active Users: [number]
   - Average Posts per User: [x.xx]
   - Most Active User: [@username] with [x] posts

2. Engagement Metrics:
   - Average Engagement Rate: [x.xx]%
   - Most Engaging Post: "[post preview]..." with [x] interactions
   - Average Interactions per Post:
     - Likes: [x.xx]
     - Comments: [x.xx]
     - Shares: [x.xx]

3. Content Analysis:
   - Total Hashtags: [number]
   - Top 5 Trending Hashtags:
     1. #[hashtag1] ([count])
     2. #[hashtag2] ([count])
     ...
   - Post Types:
     - Text: [x]%
     - Image: [x]%
     - Video: [x]%
     - Other: [x]%

4. Temporal Analysis:
   - Peak Activity Hours: [time] - [time]
   - Posts by Time of Day:
     - Morning (6AM-12PM): [x]%
     - Afternoon (12PM-5PM): [x]%
     - Evening (5PM-10PM): [x]%
     - Night (10PM-6AM): [x]%

5. User Interactions:
   - Total Comments: [number]
   - Most Active Commenter: [@username] with [x] comments
   - Post with Most Discussion: "[post preview]..." with [x] comments
```

## 💡 Hints

- Use `find_all()` with specific class names to locate posts and comments
- Handle relative timestamps (e.g., "2 hours ago") by converting to datetime objects
- Use regular expressions to extract hashtags and mentions
- For engagement rate, consider: (likes + comments + shares) / impressions * 100
- Handle pagination or infinite scroll if present in the HTML
- Use `json` module to work with any embedded JSON data in the page

## 🧪 Testing Your Solution

Verify that:
- All posts and their metadata are correctly extracted
- The engagement metrics are calculated accurately
- The analysis handles edge cases (posts without comments, deleted users, etc.)
- The solution works with the full range of post types and formats

## 📝 Notes

- The HTML structure may be complex with many nested elements
- Some data might be loaded dynamically via JavaScript
- Pay attention to how images and videos are embedded
- Consider the ethical implications of web scraping social media data

## 📚 Additional Resources

- [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Python Regular Expressions](https://docs.python.org/3/library/re.html)
- [DateTime Module](https://docs.python.org/3/library/datetime.html)
- [JSON Module](https://docs.python.org/3/library/json.html)

Happy Scraping! 📱
