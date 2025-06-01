
# 🛡️ SQLI Guard - Advanced AI-Powered SQL Injection Protection

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Gradio](https://img.shields.io/badge/interface-Gradio-FF4B4B.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg)


**SQLI Guard** is a comprehensive, AI-powered tool designed to detect, analyze, visualize, and prevent SQL injection attacks. It leverages advanced machine learning models (BERT, GAN, Stable Diffusion), natural language processing, and interactive visualizations to provide robust cybersecurity analysis and protection for SQL queries. The tool includes a Gradio-based web interface for intuitive user interaction, making it suitable for developers, security researchers, and red teamers.

## Features

- **AI-Powered Detection**: BERT-based classification of SQL queries
- **Interactive Visualizations**: 3D pattern analysis, heatmaps, and network graphs
- **Protection Tools**: Query sanitization and parameterization
- **Red Team Simulation**: Generate adversarial SQL injection examples
- **Honeypot Simulation**: Simulate attack scenarios
- **Natural Language to SQL**: Convert plain English to secure SQL
- **Voice Interface**: Voice-to-SQL conversion
- **Stable Diffusion Integration**: Generate attack story visuals
- **Community Pattern Library**: Crowdsourced detection patterns

## Installation


### Prerequisites
- Python 3.8+
- CUDA-enabled GPU (optional, for faster computation with PyTorch)
- Groq API key (sign up at [x.ai/api](https://x.ai/api))
- FFmpeg (for audio processing, required for voice-to-SQL)

1. Clone the repository:
```bash
git clone https://github.com/JaanuNan/sqli-guard.git
cd sqli-guard
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up your Groq API key (for LLM features):
```bash
export GROQ_API_KEY="your-api-key-here"
```

## Usage

Run the Gradio interface:
```bash
python app.py
```

The web interface will launch at `http://localhost:7860` with these main components:


- **Query Analysis**:Enter a SQL query in the "Query Analysis" tab.Select the database type (generic, MySQL, PostgreSQL) and image style (comic-strip, cyberpunk, realistic).Click "Analyze Query" to view classification, confidence scores, visualizations, sanitized query, and threat analysis.
- **Protection Tools**:Review sanitized and parameterized queries.Explore the attack DNA network graph for pattern analysis.
- **Honeypot Simulation**:Run simulations to generate mock attack data and visualize classification results.
- **Red Team Simulator**:Generate adversarial SQL queries by selecting an attack type (basic, blind, obfuscated, etc.).Analyze the complexity of generated queries.
- **Voice-to-SQL**:Upload an audio file or record a natural language query.Convert it to a secure SQL query with accompanying visualizations and CSV export.
- **Community Patterns**:Submit new SQL injection patterns with descriptions and severity levels.View the community pattern library in a table format.
- **Security Assistant**:Interact with AskSQLiBot to ask questions about SQL injection prevention and best practices.

## Screenshots

![Query Analysis](screenshots/analysis.png)
*Query analysis with 3D visualization*

![Honeypot Simulation](screenshots/honeypot.png)
*Honeypot attack simulation*

## Technical Components

- **Machine Learning**: BERT model fine-tuned for SQLi detection
- **Visualization**: Plotly for interactive 3D and 2D charts
- **Natural Language Processing**: Groq/Llama for explanations
- **Adversarial Generation**: GAN for attack pattern generation
- **Voice Interface**: Whisper-based speech recognition

## Requirements

See [requirements.txt](requirements.txt) for full dependency list.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact
Project Link: [https://github.com/JaanuNan/sqli-guard.git](https://github.com/JaanuNan/sqli-guard.git)

## Acknowledgments

- Built with Gradio for the interactive UI.
- Powered by Hugging Face Transformers for BERT and Stable Diffusion.
- Leverages Groq API for NLP and transcription.
- Visualizations created with Plotly and NetworkX.

### Notes:


1. For the Stable Diffusion model, you may want to add `xformers` for better performance if using CUDA
2. Consider adding a `.env.example` file for environment variables
3. You might want to add a `setup.py` for pip installation if you plan to package this

Protect your applications from SQL injection with SQLI Guard!

