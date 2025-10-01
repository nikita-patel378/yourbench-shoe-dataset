# YourBench Shoe Knowledge Dataset

A synthetic question-answering dataset generated from research papers focused on biomechanics using the [YourBench](https://github.com/huggingface/yourbench) framework.

## Overview

This project uses YourBench, an open-source framework for generating synthetic datasets from PDFs, to create diverse question-answering pairs focused on shoe knowledge and footwear science. The framework leverages LLMs to generate various types of questions based on the content of research papers.

## Features

- Generates diverse question types (factual, reasoning, application-based, etc.)
- Customizable LLM selection for dataset generation
- Outputs ready for fine-tuning language models
- Direct push to HuggingFace for easy sharing and use

## Setup

1. Clone this repository
2. Install YourBench dependencies (see [YourBench documentation](https://github.com/huggingface/yourbench))
3. Download the source papers listed in `sources/README.md` and place them in a `data/` folder to define a path for the yaml file.
4. Set environmental variables (specifically for LLM and HF_TOKEN. HF_ORGANISATION is optional)
5. Configure your LLM settings in `config.yaml`. For LLM I used google/gemini-2.5-flash through OpenRouter

## Usage

Run YourBench with the provided configuration:
```
yourbench config.yaml
