# Twitter_Query_Analysis
Step 1: Install Python and Required Libraries
Step 2: Prepare the Dataset
Step 3: Convert created_at to DateTime Format
Step 4: Run the Query Function

# Key Design Choices
1. Pandas for Data Handling:
We use pandas to handle the dataset because it is fast, well-documented, and easy to use for data analysis and manipulation.

2. Search Functionality:
The system filters tweets that contain a specific term, allowing for flexible searches. We use str.contains() to check if the term appears in the tweet's text.

3. Datetime Conversion:
Converting the created_at column to datetime with utc=True is crucial to correctly handling timezone-aware timestamps. This ensures consistent time-based queries (e.g., by day, hour).

4. Efficient Grouping:
We group tweets by day, hour, and users efficiently using groupby(), which is optimized for performance with large datasets.

5. User-Focused Results:
We provide actionable insights (e.g., the most active user, average likes) to help users quickly understand trends.
