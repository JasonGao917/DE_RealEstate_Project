# Real Estate E2E Data Engineering

## Project Overview
This project demonstrates an end-to-end real estate data engineering pipeline using various technologies including AI, web scraping, streaming, and big data storage. The pipeline collects real estate listings from Zoopla, processes the data using a large language model, streams the data into Kafka, and stores it in Cassandra via Spark.

## Architecture
1. **BrightData WebScraper**: Scrapes real estate listing data from Zoopla.
2. **Language Model Processing**: Utilizes a large language model to parse and structure the scraped data.
3. **Kafka Streaming**: Streams the processed data into Kafka, managed by ZooKeeper, and visualized using Control Center.
4. **Spark Processing**: The Spark master collects data from Kafka and distributes tasks to workers.
5. **Data Storage**: Spark workers store the processed data into a Cassandra database.

## Components
- **Kafka and ZooKeeper**: Manages and streams data.
- **Spark**: Processes and distributes the data workload.
- **Cassandra**: Stores the structured data for further analysis.
- **Playwright and Beautiful Soup**: Tools used in the scraping process to interact with and parse web content.
- **OpenAI GPT**: Provides AI capabilities for processing the data.
