# Zillow Data Engineering Pipeline

![Pipeline Overview](./assets/pipeline-overview.png)

## Overview

This project demonstrates a comprehensive data engineering solution that starts with fetching real estate listings from Zillow using its API, and then efficiently processes and manages this data through a structured flow involving a data lake, data warehouse, and a final ETL (Extract, Transform, Load) operation. The end product is a clean, processed CSV data which gets loaded into an Amazon Redshift database.

## Table of Contents

- [Project Highlights](#project-highlights)
- [Architecture](#architecture)
- [Prerequisites](#prerequisites)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Project Highlights

1. **Zillow API Integration**: Seamless integration with Zillow's API to fetch fresh real estate listings.
2. **Data Lake Formation**: Temporary storage allowing for data exploration, analytics, and further processing.
3. **Data Warehousing**: Structured data management ensuring scalability and reliability.
4. **ETL Processing**: Converting complex JSON data into user-friendly CSV format.
5. **Amazon Redshift Integration**: Data storage solution making querying efficient and easy.

## Architecture

The pipeline follows a structured flow:

1. **Data Extraction**: Using Zillow API to get the listings in JSON format.
2. **Data Lake**: Store the raw JSON in an S3 bucket allowing for flexibility and scalability.
3. **Data Warehouse**: Further processing and management using AWS solutions.
4. **ETL Process**: The data is then transformed from JSON to CSV and loaded into Redshift.

## Prerequisites

- An AWS Account
- Configured AWS CLI
- Zillow API Key

## Setup and Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your_username/Zillow-Data-Engineering-Pipeline.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd Zillow-Data-Engineering-Pipeline
    ```

3. **Set up the required environment variables**:
    - AWS_ACCESS_KEY_ID
    - AWS_SECRET_ACCESS_KEY
    - ZILLOW_API_KEY

4. **Execute the setup script** (this will set up necessary resources on AWS and configure other required settings):
    ```bash
    ./setup.sh
    ```

## Usage

To start the data engineering pipeline:

```bash
python run_pipeline.py
```

## Contributing
Many thanks to [@tuplespectra](https://www.youtube.com/@tuplespectra) for providing an in-depth example that established the base pipeline for this project.

