# Health Analytics Case Study <img src="/IMG/pngwing.com.png" align="right" width="120" />

> This case study is contained within the [Serious SQL](https://www.datawithdanny.com) by [Danny Ma](https://www.linkedin.com/in/datawithdanny/)
> 
## 📕 **Table of contents**
<!--ts-->
   * 🛠️ [Overview](#️-overview)
   * 🚀 [Solutions](#-solutions)
   * 💻 [Key Highlights](#-key-highlight)


## 🛠️ Overview
With the **Health Analytics Mini Case Study**, I queried data to bring insights to the following questions:
1. How many `unique users` exist in the logs dataset?
2. How many total `measurements` do we have `per user on average`?
3. What about the `median` number of measurements per user?
4. How many users have `3 or more` measurements?
5. How many users have `1,000 or more` measurements?
6. Have logged `blood glucose` measurements?
7. Have `at least 2 types` of measurements?
8. Have all 3 measures - `blood glucose, weight and blood pressure`?
9. What is the `median systolic/diastolic` **blood pressure** values?

---
## 🚀 Solutions
![Question 1](https://img.shields.io/badge/Question-1-971901)
### **How many unique users exist in the logs dataset?**
```sql
SELECT COUNT (DISTINCT id)
FROM health.user_logs;
```

|count                                   |
|----------------------------------------|
|554                                     |
