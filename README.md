# Social Network Data Analysis

## Project Overview

This project analyzes large-scale social network datasets (1M+ rows per table) using SQL to answer key questions about user engagement, friend activity, and messaging behavior. The analysis demonstrates advanced querying techniques including joins, aggregations, filtering, and subqueries to extract meaningful insights from relational databases.

---

## Project Objectives

Identify the user with the highest number of friends in the network.

Determine the top users who send the most friend requests.

Calculate the number and percentage of accepted friend requests.

Analyze messaging activity, including keyword frequency in messages.

Detect users with more than 10 unread messages to evaluate engagement and responsiveness.

---

## Methodology

User and Friend Request Analysis

Queried the users table to find the maximum friend_count and the corresponding user email.

Joined users and friend_requests tables to identify the top three users sending the most requests.

Friend Request Acceptance Evaluation

Counted all accepted friend requests from the friend_requests table.

Calculated the percentage of accepted requests relative to total requests using nested subqueries.

Messaging Analysis

Queried the messages table to count messages containing the phrase "Miss you" using case-insensitive pattern matching.

Grouped messages by sender to identify users with more than 10 unread messages (date_read IS NULL).

Data Aggregation and Summarization

Used COUNT(), MAX(), and GROUP BY to aggregate activity metrics.

Applied filtering and HAVING clauses to detect high-activity or high-engagement users.

Validation and Accuracy

Checked query results for logical consistency and ensured metrics matched expected patterns in large datasets (1M+ rows).

---

## Key Findings

Most Connected User: Identified the user with the highest friend count, providing insights into the platform’s most connected members.

Top Friend Request Senders: Determined the three most active users initiating friend requests, highlighting power users driving engagement.

Friend Request Acceptance Rate: Calculated the total number of accepted requests and found the percentage relative to all requests, revealing overall user connectivity success.

Messaging Behavior: Counted all messages containing the phrase "Miss you", providing insight into engagement and user sentiment.

Unread Messages: Identified users with more than 10 unread messages, pinpointing potential areas for engagement improvement or system notifications.

---

## Dataset Description

The project uses three relational tables:

users – user profile data including email, username, friend count

friend_requests – friend request records with requester, requestee, and status

messages – message logs between users

Each table contains 1M+ rows, simulating real-world large-scale social network data.

---

## Analysis Questions
1. User with the Most Friends

Identified the email and friend count of the most connected user using a subquery with MAX(friend_count).

2. Most Active Friend Request Senders

Joined users and friend_requests tables to find the top 3 users who sent the most friend requests.

3. Friend Request Acceptance Rate

Counted accepted friend requests

Calculated the percentage of accepted requests across the platform

4. Message Keyword Analysis

Counted messages containing the phrase “Miss you” using case-insensitive filtering.

5. High Unread Message Users

Identified users with more than 10 unread messages using grouping and HAVING.

---

## Key Insights Demonstrated

Ability to analyze large datasets efficiently with SQL

Experience working with relational joins and aggregations

Understanding of user engagement metrics

Ability to calculate behavioral trends and platform KPIs

---

## Skills Demonstrated

SQL Querying: Writing complex queries using SELECT, JOIN, GROUP BY, HAVING, and subqueries.

Data Aggregation & Summarization: Calculating counts, maximums, percentages, and conditional aggregations for user and messaging metrics.

Data Filtering & Pattern Matching: Using WHERE, LIKE, and conditional logic to extract meaningful subsets of data.

Large Dataset Management: Efficiently analyzing tables with 1M+ rows to generate actionable insights.

Relational Database Analysis: Understanding relationships between tables and leveraging joins to combine user, friend request, and messaging data.

Behavioral & Engagement Metrics: Measuring user activity, friend request acceptance, unread messages, and messaging patterns.

Data Cleaning Awareness: Handling null values and identifying data inconsistencies to ensure query accuracy.

---

## Tools Used

SQLite

SQL (JOIN, GROUP BY, Subqueries, Filtering)
