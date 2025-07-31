# 🤖 MCP Learning Path Generator

An intelligent learning path generator that uses Model Context Protocol (MCP) to create personalized, day-wise learning journeys by combining YouTube content with Google Drive or Notion integration.

## 🚀 Features

- **AI-Powered Learning Paths**: Generate comprehensive, structured learning paths using Google's Gemini 2.5 Flash model
- **YouTube Integration**: Automatically search and curate relevant YouTube videos for each learning topic
- **Document Creation**: Create organized learning documents in Google Drive or Notion
- **Playlist Generation**: Automatically create YouTube playlists with curated content
- **Real-time Progress Tracking**: Visual progress indicators during generation
- **Multiple Tool Support**: Choose between Google Drive or Notion for document storage

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **AI Model**: Google Gemini 2.5 Flash
- **Protocol**: Model Context Protocol (MCP)
- **Tools**: YouTube API, Google Drive API, Notion API
- **Framework**: LangChain + LangGraph

## 📋 Prerequisites

Before running this application, you'll need:

1. **Google API Key**: For accessing Gemini AI model
2. **Pipedream URLs**: For YouTube, Google Drive, and/or Notion integrations
3. **Python 3.8+**: For running the application

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd mcp-learning-path-demo-main
```

### 2. Set Up Virtual Environment

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run app.py
```

The application will open in your default browser at `http://localhost:8501`

## ⚙️ Configuration

### Required Setup

1. **Google API Key**: 
   - Get your API key from [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Enter it in the sidebar when the app loads

2. **YouTube Pipedream URL** (Required):
   - Set up a Pipedream workflow for YouTube API
   - Enter the URL in the sidebar

### Optional Setup

3. **Secondary Tool** (Choose one):
   - **Google Drive**: Set up Pipedream workflow for Google Drive API
   - **Notion**: Set up Pipedream workflow for Notion API
   - Enter the corresponding URL in the sidebar

## 📖 How to Use

1. **Configure APIs**: Enter your Google API key and required URLs in the sidebar
2. **Select Tools**: Choose between Google Drive or Notion for document storage
3. **Enter Learning Goal**: Describe what you want to learn, for example:
   - "I want to learn Python basics in 3 days"
   - "I want to learn data science fundamentals in 10 days"
   - "I want to master web development in 2 weeks"
4. **Generate Path**: Click "Generate Learning Path" and watch the AI create your personalized learning journey
5. **Access Results**: Get links to your created document and YouTube playlist

## 🔧 Project Structure

```
mcp-learning-path-demo-main/
├── app.py              # Main Streamlit application
├── utils.py            # Core agent setup and execution logic
├── prompt.py           # AI prompt templates
├── requirements.txt    # Python dependencies
└── README.md          # This file
```

## 🧠 How It Works

1. **Agent Setup**: The application initializes an MCP client with configured tools (YouTube, Drive/Notion)
2. **Goal Processing**: Your learning goal is processed by the AI to create a structured plan
3. **Content Research**: The AI searches YouTube for relevant educational content
4. **Document Creation**: A comprehensive learning path document is created in your chosen platform
5. **Playlist Generation**: A curated YouTube playlist is created with the selected videos
6. **Result Delivery**: You receive links to both the document and playlist

## 📝 Example Output

The generated learning path includes:
- **Day-wise structure** with clear topics
- **YouTube video links** for each learning session
- **Organized document** in Google Drive or Notion
- **Curated YouTube playlist** for easy access
- **Additional resources** and channel recommendations

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Streamlit](https://streamlit.io/) for the web interface
- Powered by [Google Gemini](https://ai.google.dev/) for AI capabilities
- Uses [Model Context Protocol](https://modelcontextprotocol.io/) for tool integration
- Integrates with [YouTube](https://www.youtube.com/), [Google Drive](https://drive.google.com/), and [Notion](https://www.notion.so/) APIs

## 📞 Support

If you encounter any issues or have questions:
1. Check the [Issues](https://github.com/yourusername/your-repo/issues) page
2. Create a new issue with detailed information
3. Include error messages and steps to reproduce

---

**Happy Learning! 🎓**
