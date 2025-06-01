
# 🛡️ SQLI Guard - Advanced AI-Powered SQL Injection Protection

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Gradio](https://img.shields.io/badge/interface-Gradio-FF4B4B.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg)

SQLI Guard is an advanced AI-powered toolkit for detecting, visualizing, and preventing SQL injection attacks. It combines machine learning models with interactive visualizations to provide comprehensive SQL injection protection.

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

1. **Query Analysis**: Enter SQL queries for detection and visualization
2. **Protection Tools**: View sanitized and parameterized queries
3. **Honeypot Simulation**: Simulate attack scenarios
4. **Security Assistant**: Chat with an AI security expert
5. **Red Team Simulator**: Generate adversarial queries
6. **Voice Interface**: Convert spoken queries to secure SQL

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
### Notes:


1. For the Stable Diffusion model, you may want to add `xformers` for better performance if using CUDA
2. Consider adding a `.env.example` file for environment variables
3. You might want to add a `setup.py` for pip installation if you plan to package this

