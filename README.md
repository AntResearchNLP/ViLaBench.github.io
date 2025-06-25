# ViLaBench
**Please directly see https://antresearchnlp.github.io/vilabench/ for visualization of the benchmark collection.**

This is a web project showcasing a collection of benchmarks for vision-language models.

These benchmark and result data are carefully compiled and merged from technical reports and official blogs of renowned multimodal models, including Google's Gemini series ([Gemini 2.5 Report](https://storage.googleapis.com/deepmind-media/gemini/gemini_v2_5_report.pdf)), OpenAI GPT series and OpenAI o series ([OpenAI o3 and o4-mini](https://openai.com/index/introducing-o3-and-o4-mini/)), [Seed1.5-VL](https://arxiv.org/pdf/2505.07062), [MiMo-VL](https://arxiv.org/pdf/2506.03569), [Kimi-VL](https://huggingface.co/moonshotai/Kimi-VL-A3B-Thinking-2506), [Qwen2.5-VL](https://arxiv.org/pdf/2502.13923), [InternVL3](https://arxiv.org/abs/2504.10479), and other leading models' official technical documentation.

This collection provides researchers and developers with a comprehensive, standardized multimodal model evaluation benchmark comparison platform, helping to advance the development and research in the vision-language model field. Through unified data formats and visualization interfaces, users can more intuitively understand the performance of different models on various tasks, providing valuable references for model selection and improvement.

## Features

- 📊 **Dynamic Data Display**: Automatically reads and displays data from vilabench.csv
- 🔍 **Search and Filter**: Support searching by benchmark name, task, domain, etc.
- 🏷️ **Smart Tags**: Automatically converts image, multiple image, video to visual tags
- 🔗 **Link Navigation**: Benchmark names are clickable and link to corresponding papers
- 📱 **Responsive Design**: Supports both desktop and mobile devices
- 📈 **Statistics**: Real-time display of data statistics

## Local Usage

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
