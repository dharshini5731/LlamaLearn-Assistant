# 🦙 LlamaLearn Assistant

An AI-powered interactive learning platform that transforms your study notes into engaging quizzes, flashcards, and provides comprehensive learning analytics. Built with Streamlit and powered by Groq's Llama models.

## ✨ Features

### 🎯 Core Learning Tools
- **📤 PDF Upload**: Upload your study notes in PDF format
- **🤔 AI Q&A**: Ask questions about your uploaded notes and get detailed answers
- **📋 Interactive Quizzes**: Auto-generated quizzes with multiple choice and true/false questions
- **🃏 Smart Flashcards**: AI-generated flashcards with difficulty levels
- **📈 Performance Analytics**: Detailed progress tracking with visual charts

### 🚀 Advanced Features
- **🔥 Learning Streaks**: Track daily study habits and maintain streaks
- **🏆 Leaderboard**: Compete with other learners and see rankings
- **📊 Interactive Analytics**: Comprehensive performance dashboards with charts
- **🎨 Difficulty Levels**: Adaptive content based on easy/medium/hard levels
- **👥 Multi-user Support**: User authentication and role-based access
- **🛡️ Admin Panel**: Administrative dashboard for platform management

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **AI/ML**: Groq API with Llama-3 70B model
- **Document Processing**: LangChain, PyPDF2
- **Data Visualization**: Plotly, Pandas
- **Data Storage**: JSON-based local storage
- **Authentication**: Custom user management system

## 📋 Prerequisites

- Python 3.8 or higher
- Groq API key (get it from [Groq Console](https://console.groq.com/))

## 🚀 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/llamalearn-assistant.git
cd llamalearn-assistant
```

### 2. Create Virtual Environment (Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Set Up Groq API Key
Edit the `enhanced_aitutor1.py` file and replace the API key:
```python
os.environ["GROQ_API_KEY"] = "your_groq_api_key_here"
```

**⚠️ Security Note**: For production use, set the API key as an environment variable:
```bash
export GROQ_API_KEY="your_groq_api_key_here"
```

### 5. Run the Application
```bash
streamlit run enhanced_aitutor1.py
```

The application will open in your browser at `http://localhost:8501`

## 📚 Usage Guide

### Getting Started
1. **Register**: Create a new account or use the default login
2. **Upload Notes**: Upload your study materials in PDF format
3. **Start Learning**: Choose from quizzes, flashcards, or Q&A sessions

### User Roles
- **Student**: Access to all learning features
- **Admin**: Additional access to analytics dashboard and user management

### Default Admin Account
- Username: `admin`
- Password: `admin123`
- Role: `admin`

## 🎮 Features Walkthrough

### 📤 Upload Notes
- Support for PDF documents
- Automatic text extraction and processing
- Content validation and preprocessing

### 🤔 Ask Questions
- Natural language queries about your notes
- AI-powered contextual answers
- Real-time response generation

### 📋 Interactive Quiz
- Multiple choice and True/False questions
- Customizable difficulty levels (easy/medium/hard)
- Progress tracking and review mode
- Detailed explanations for each answer

### 🃏 Flashcards
- AI-generated question-answer pairs
- Difficulty-based filtering
- Session tracking and accuracy metrics
- Spaced repetition learning

### 📈 Performance Analytics
- Learning progress visualization
- Accuracy trends over time
- Study activity heatmaps
- Streak tracking and session history

### 🏆 Leaderboard
- User rankings based on performance
- Comparative analytics
- Streak competitions
- Community engagement features

## 📊 Data Storage

The application uses JSON files for data persistence:

- `users.json`: User authentication data
- `learning_data.json`: Learning sessions and performance metrics
- `temp.pdf`: Temporary storage for uploaded PDFs

## 🔧 Configuration

### Customizing Quiz Settings
- Number of questions: 5, 10, 15, or 20
- Question types: Multiple Choice, True/False, or Mixed
- Difficulty levels: Easy, Medium, Hard, or Mixed

### Performance Metrics
- Session accuracy tracking
- Daily learning streaks
- Total questions attempted
- Time-based progress analytics

## 🚨 Troubleshooting

### Common Issues

1. **API Key Errors**
   - Ensure your Groq API key is valid and properly set
   - Check API rate limits and quotas

2. **PDF Upload Issues**
   - Verify PDF is not password-protected
   - Ensure PDF contains extractable text (not scanned images)

3. **Missing Dependencies**
   - Run `pip install -r requirements.txt` to install all dependencies
   - Use virtual environment to avoid conflicts

4. **Port Already in Use**
   - Use a different port: `streamlit run enhanced_aitutor1.py --server.port 8502`

### Debug Mode
Add `--logger.level=debug` to the streamlit command for verbose logging:
```bash
streamlit run enhanced_aitutor1.py --logger.level=debug
```

## 🔒 Security Considerations

- **API Keys**: Never commit API keys to version control
- **User Data**: Implement proper data encryption for production use
- **Authentication**: Consider implementing OAuth or JWT for enhanced security
- **Data Privacy**: Ensure compliance with data protection regulations

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow PEP 8 style guidelines
- Add docstrings to functions
- Include error handling for external API calls
- Test new features thoroughly

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Groq](https://groq.com/) for providing the AI inference API
- [Streamlit](https://streamlit.io/) for the web application framework
- [LangChain](https://langchain.com/) for document processing capabilities
- [Plotly](https://plotly.com/) for interactive visualizations

## 📞 Support

For support and questions:
- Create an issue on GitHub
- Check the troubleshooting section above
- Review the Groq documentation for API-related issues

## 🚀 Future Enhancements

- [ ] Mobile-responsive design
- [ ] Multiple file format support (DOCX, TXT, etc.)
- [ ] Voice-based interaction
- [ ] Advanced spaced repetition algorithms
- [ ] Integration with external learning platforms
- [ ] Real-time collaborative features
- [ ] Advanced analytics and insights
- [ ] Export capabilities for study materials

---

**Happy Learning! 🎓**
