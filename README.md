# Intelligent-Customer-Support-Agent-with-LangGraph 

## Overview  
This project demonstrates how to build an AI-powered customer support agent using **LangGraph**, a tool for designing and managing complex language model workflows. The agent automates query categorization, sentiment analysis, response generation, and escalation of critical issues to human agents, showcasing the power of AI and graph-based workflows.  

## Motivation  
Efficient customer support is crucial in today's fast-paced business world. Automating initial customer interactions can reduce response times and improve satisfaction. This project highlights how language models and graph workflows can create a scalable and sophisticated support system for handling diverse inquiries.  

## Key Features  
- **Query Categorization**: Classifies queries as Technical, Billing, or General.  
- **Sentiment Analysis**: Identifies the emotional tone of customer queries (Positive, Neutral, Negative).  
- **Response Generation**: Provides relevant responses tailored to the query's category and sentiment.  
- **Escalation Mechanism**: Routes critical or negative queries to human agents.  
- **Graph Workflow**: Utilizes LangGraph for building scalable and extensible workflows.  

## Methodology  

1. **State Management**: Use `TypedDict` to manage customer interaction data.  
2. **Node Functions**: Implement stages like query categorization, sentiment analysis, and response generation.  
3. **Workflow Graph**: Create a graph using LangGraph to represent the customer support process.  
4. **Conditional Routing**: Route queries based on category and sentiment using dynamic logic.  
5. **Execution**: Process queries through the compiled workflow to generate results.  

## Installation  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/customer-support-agent-langgraph.git
   cd customer-support-agent-langgraph
   ```  
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  
3. Set your OpenAI API key in a `.env` file:  
   ```plaintext
   OPENAI_API_KEY=your-api-key
   ```  

## Usage  

1. Import necessary libraries and load environment variables.  
2. Define the customer interaction state structure.  
3. Implement functions for query categorization, sentiment analysis, and responses.  
4. Create and configure the LangGraph workflow.  
5. Run customer queries through the workflow using the `run_customer_support()` function.  

### Example Queries  

#### Input:  
- **Query**: "What are your business hours?"  
#### Output:  
- **Category**: General  
- **Sentiment**: Neutral  
- **Response**: "Our business hours are [insert hours]. Feel free to contact us during this time."  

## Visualization  
LangGraph workflows can be visualized using Mermaid diagrams to better understand the process.  

```python
from IPython.display import display, Image
display(
    Image(
        app.get_graph().draw_mermaid_png(draw_method=MermaidDrawMethod.API)
    )
)
```  

## Conclusion  
This project showcases how LangGraph can simplify the orchestration of AI-driven customer support workflows. It is a scalable, adaptable solution with potential applications beyond customer support, making it an excellent starting point for businesses looking to enhance efficiency and improve user satisfaction.  

Feel free to customize and extend this workflow for your specific business needs!  

## License  
This project is licensed under the MIT License.  
```
