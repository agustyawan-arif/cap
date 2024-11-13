### Quis:
Google form url for quis and case submission: https://forms.gle/YJYBNXdsghiuu8uW7

### Case Study: Customer Support Assistant

**Scenario:**  
You are developing an AI-powered customer support assistant using LangChain and OpenAI. The assistant should help customers with various requests, such as providing product information, offering solutions to common issues, and summarizing product reviews. The goal is to build a system that can handle different types of requests and provide structured, actionable responses.

**Task:**  
Using LangChain, implement the following functionalities for the assistant:

1. **Product Inquiry Response**  
   - Create a prompt where a customer inquires about a specific product, such as: *"Tell me more about the features of the latest smartphone model."*
   - The model should respond with key features of the product in a structured format using Pydantic. Define fields such as `product_name`, `features`, and `price_range`.
   - Display each part of the response separately.

2. **Troubleshooting Assistance**  
   - The assistant should respond to common troubleshooting questions, like: *"My smartphone isn’t charging. What could be the issue?"*
   - Use a chaining approach to first identify the problem and then provide two possible solutions. For instance, one suggestion could be checking the charging cable, and another could be restarting the device.
   - Print both the identified issue and the suggested solutions.

3. **Review Summarization with Sentiment Analysis**  
   - Customers often leave reviews. Ask the model to summarize a sample review, like: *"The phone is good, but the battery life could be better."*
   - Generate a structured output where the assistant categorizes the review summary and identifies the sentiment as either *positive*, *neutral*, or *negative*.
   - Print the review summary and the detected sentiment.

4. **Usage Monitoring and Token Tracking**  
   - To manage API costs, monitor the total tokens used across all tasks in this assistant.
   - Use the callback function to track the tokens and display the total usage after all tasks are completed.
   - Output in USD and IDR

### Example Output

For **Product Inquiry Response**:
```plaintext
Product Name: Latest Smartphone
Features: ["High-resolution camera", "Fast charging", "OLED display"]
Price Range: "$699 - $999"
```

For **Troubleshooting Assistance**:
```plaintext
Issue: Device not charging
Solutions: 
1. Check the charging cable.
2. Restart the device.
```

For **Review Summarization with Sentiment Analysis**:
```plaintext
Review Summary: The phone is good, but the battery life could be better.
Sentiment: Neutral
```

For **Token Usage**:
```plaintext
Total tokens used: $150 or IDR 2336100
```
