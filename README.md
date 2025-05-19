# AI-Powered-task-Management-system
 AI-powered system to classify and prioritize Jira tasks using ML
# AI-Powered Task Management System

An intelligent task management system that uses AI to automate task classification, prioritization, and assignment.

## Features

- Task Classification using NLP and ML
- Priority Prediction
- Workload Balancing
- Jira Integration
- RESTful API
- Docker Support

## Project Structure

```
.
├── app/
│   ├── api/            # FastAPI routes
│   ├── core/           # Core application logic
│   ├── models/         # ML models
│   ├── services/       # Business logic
│   └── utils/          # Utility functions
├── config/             # Configuration files
├── data/              # Data storage
├── notebooks/         # Jupyter notebooks
├── tests/             # Test files
├── Dockerfile         # Docker configuration
├── requirements.txt   # Project dependencies
└── README.md         # Project documentation
```

## Setup

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up environment variables:
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

## Running the Application

### Development
```bash
uvicorn app.main:app --reload
```

### Production (Docker)
```bash
docker build -t ai-task-manager .
docker run -p 8000:8000 ai-task-manager
```

## API Documentation

Once the application is running, visit:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Testing

```bash
pytest
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

MIT License
