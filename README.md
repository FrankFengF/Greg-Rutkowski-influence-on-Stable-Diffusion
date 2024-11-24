# Greg-Rutkowski-influence-on-Stable-Diffusion
Use LAION Score to quantify Greg Rutkowski's contribution on Stable Diffusion

# Overview
The project is designed to process and analyze prompts and images, specifically focusing on modifications related to artist references, such as Greg Rutkowski, and generating metrics to evaluate the aesthetic or stylistic qualities of images. This is part of a larger workflow for understanding the impact of artist-specific terms in AI-generated content.

# Key Features
## 1. Prompt Extraction and Cleaning
Extracts 1,200 prompts from the DiffusionDB metadata.


Cleans prompts by removing non-English characters.


Strips mentions of "Greg Rutkowski," including common misspellings like "Rukowski."
## 2. Image Generation
Utilizes Stable Diffusion XL (SDXL) and Stable Diffusion v1.5 models via API for image generation.


Supports specifying a range of prompts using configurable start and end indices.


Facilitates experimentation with positive, base, and negative prompting strategies

## 3. LAION Score Evaluation
Calculates LAION scores for generated images and exports results in Excel format.


Sorts scores in ascending order by decimal values (originally in binary order).


Filters out scores for black images caused by NSFW detection in SD1.5 (images scored as 3.357).

## 4. Prompt Relatedness Calculation
Analyzes Greg Rutkowski’s portfolio and uses GPT to describe his work.

Calculates the frequency of each word in the prompts.

Assigns a Lift Score to each word based on its relevance.

Computes the sum and average Lift Scores for each prompt.

# Usage Instructions
## 1. Prepare the Input Data:

Extract metadata from DiffusionDB.

Save prompts in the required format for processing.

# 2. Run the Notebook:
Open files in Jupyter Notebook or a compatible environment.

Follow the instructions in each cell to process prompts, generate images, and calculate metrics.

## 3. Analyze Results:

Review LAION scores in the provided Excel files.

Evaluate prompt relatedness metrics to understand stylistic contributions.

# Author
Created by: Qiuyang Feng, Haojie Ge, David Schweidel

Contact: frank.feng2@emory.edu, haojie.ge@emory.edu, dschweidel@emory.edu
