# ViLaBench

This is a web project showcasing collection of benchmarks for vision-language models.

## Features

- 📊 **Dynamic Data Display**: Automatically reads and displays data from vilabench.csv
- 🔍 **Search and Filter**: Support searching by benchmark name, task, domain, etc.
- 🏷️ **Smart Tags**: Automatically converts image, multiple image, video to visual tags
- 🔗 **Link Navigation**: Benchmark names are clickable and link to corresponding papers
- 📱 **Responsive Design**: Supports both desktop and mobile devices
- 📈 **Statistics**: Real-time display of data statistics

## Usage

1. Ensure `vilabench.csv` and `index.html` are in the same directory
2. Use a local server to open the webpage (to avoid CORS issues):
   ```bash
   python3 -m http.server 8000
   ```
3. Visit `http://localhost:8000` in your browser

## Data Format

The CSV file contains the following columns:
- Benchmark: Benchmark name
- URL: Paper link
- year: Publication year
- cognitive levels: Cognitive level
- category: Category
- domain: Domain
- task: Task type
- image: Whether it supports images
- multiple image: Whether it supports multiple images
- video: Whether it supports videos
- score: Model scores (JSON format)

## GitHub Pages Deployment

This project is configured for GitHub Pages and can be accessed directly at: https://antresearchnlp.github.io/vilabench
