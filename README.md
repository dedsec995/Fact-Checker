# Research Bot with GPT-4 LangChain Agents
Research Bot is an AI-powered tool designed to assist users in generating academic research reports based on their input. The bot leverages various language models and tools to provide a comprehensive research report, including introductions, quantitative facts, recent publications, recommended readings, and YouTube links related to the user's query.

## Features
- Dynamic Research Generation: Generate academic research reports based on user input.
- Multiple Research Tools: Utilize Wikipedia, DuckDuckGo, YouTube, Pubmed, and more for comprehensive research.
- Conversational Mode: Chat with the bot to refine the research and gather additional insights.
- Previous Research Retrieval: Access and render previously generated research reports.

## Technologies Used

- Python: Programming language used for the backend development.
- Streamlit: Framework for building interactive web applications.
- LangChain: Library for managing language models, tools, and memory in AI agents.
- OpenAI's GPT-3.5 Turbo: Advanced language model for text generation and understanding.
- SQLite: Database management system for storing research data.
- Pandas: Library for data manipulation and analysis.
- YouTubeSearchPython: Library for searching YouTube videos.
- dotenv: Library for loading environment variables.

## Usage
1. Generate Research:
- Enter your research query in the "User Input" text area.
- Click the "Generate Report" button to initiate the research generation process.
- The bot will generate an academic introduction, quantitative facts, recent publications, recommended readings, and YouTube links related to your query.

2. Conversational Mode:
- After generating the research report, you can chat with the bot to refine the research and gather additional insights.
- Enter your message in the "User Message" text input and click the "Submit Message" button to continue the conversation.

3. Access Previous Research:
- Switch to the "Previous Research" tab to view and render previously generated research reports.
- Select a previous user input from the dropdown menu and click the "Render Research" button to display the research details.

## Database Structure
The application uses SQLite to store research data in the `MASTER.db` database with following schema:
```sql
CREATE TABLE IF NOT EXISTS Research (
    research_id INTEGER PRIMARY KEY AUTOINCREMENT,
    user_input TEXT,
    introduction TEXT,
    quant_facts TEXT,
    publications TEXT,
    books TEXT,
    ytlinks TEXT,
    prev_ai_research TEXT
);
```

## Future Enhancements
- Allow users to uplaod their own files for research.
- Implement features like influential figures, AI scientists' perspectives, AI philosophers' perspectives, and possible routes for original research.
- Improve error handling and user feedback mechanisms.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
