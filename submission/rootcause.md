The root cause of the issues can be traced to two main areas:

Problem 1: Tags are broken up into individual characters on the post view page.
Root Cause:
Improper Handling of Tags: The tags are likely being treated as a single string without proper parsing. When displaying the tags, the string might be split into individual characters instead of being split by commas into individual tags.
Problem 2: New tags are not shown on the home page under "Popular Tags", even after a page refresh.
Root Cause:
Tag Persistence and Retrieval: When new tags are added, they might not be properly saved to the database or the popular tags list might not be updated correctly. This could be due to several reasons:
Tags are not being checked for existence and added to the "Popular Tags" collection when a new article is created.
The frontend might not be fetching the updated list of popular tags after a new article is created.
