# Mindbody's AI Strategy Generator

## Overview
This script leverages Google's GenerativeAI platform (specifically the Gemini API) to craft an AI-driven business strategy customized for Mindbody, a leader in cloud-based wellness business management software. The generated strategy is delivered in an easily digestible HTML report format.


## Requirements
- Google Colab environment
- Google account with access to GenerativeAI services
- Gemini API key obtained from [ai.google.dev](https://ai.google.dev)

## Usage
1. **Run the Script**: Execute the script in a Google Colab environment.
2. **Provide Inputs**: The script automatically sets Mindbody as the company name and provides a predefined company industry description. Enter the specific business challenge faced by Mindbody when prompted.
3. **View Generated Strategy**: The script generates an HTML report showcasing the AI-generated business strategy tailored to Mindbody and the provided challenge.
4. **Analyze and Interpret**: Review the generated strategy to gain insights and recommendations for addressing Mindbody's business challenge in the field of AI.

## Script Structure
The script consists of the following components:

### 1. `generate_business_strategy()` Function
- This function automatically sets Mindbody as the company name and provides a predefined description of the company's industry.
- It prompts the user to input the specific business challenge faced by Mindbody.
- The user input is formatted into a pre-prompt template and sent to the Gemini API for generating the business strategy.
- Returns the generated strategy text, the provided challenge, and the company name.

### 2. `generate_html_report()` Function
- Takes the generated strategy text, challenge, and company name as inputs.
- Formats the strategy into HTML format for better visualization.
- Returns the HTML content of the report.

### 3. Main Execution Flow
- Calls `generate_business_strategy()` to obtain the AI-generated strategy, challenge, and company name.
- Utilizes `generate_html_report()` to generate an HTML report based on the obtained data.
- Displays the HTML report using the `display(HTML(html_report))` function from IPython.

## Notes
- **API Key**: Ensure that you have a valid API key for accessing the Gemini API. You can obtain the API key from [ai.google.dev](https://ai.google.dev).
- **Google Colab**: This script is designed to run in a Google Colab environment due to its dependencies on Google libraries and services.
- **Input Validation**: The script currently assumes that the user will provide valid inputs for the business challenge. Additional input validation can be implemented for robustness.
- **Styling**: The HTML report is styled using CSS for better readability and presentation. You can customize the styling as needed by modifying the CSS styles within the script.
