# Docker Compose Utilities

This repository provides a centralized collection of Docker Compose configurations for various databases and services. It is designed to help developers quickly set up and experiment with different technologies in a local development environment. These configurations are not recommended for production use but are ideal for learning, testing, and prototyping.

## Project Structure

The repository is organized into folders, each containing Docker Compose configurations and related resources for a specific technology or service:

- **`cassandra-docker-compose/`**: Multi-node Cassandra cluster setup.
- **`dynamodb-docker-compose/`**: DynamoDB with DynamoDB Admin interface.
- **`elastic-docker-compose/`**: Elasticsearch and Kibana setup.
- **`influx-docker-compose/`**: InfluxDB with a pre-configured bucket.
- **`kafka-docker-compose/`**: Apache Kafka and Zookeeper configurations for single and multi-node setups.
- **`mongodb-docker-compose/`**: MongoDB with Mongo Express interface.
- **`mysql-docker-compose/`**: MySQL with a Node.js application example.
- **`postgres-docker-compose/`**: PostgreSQL with Adminer and pgAdmin interfaces.
- **`redis-docker-compose/`**: Redis Stack Server setup.
- **`splunk-docker-compose/`**: Splunk Enterprise setup.
- **`timescale-docker-compose/`**: TimescaleDB setup for time-series data.

Each folder contains:
- A `docker-compose.yml` file for setting up the service(s).
- A `README.md` file with instructions specific to the service.
- Additional resources like images or configuration files.

## Getting Started

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/docker-compose-utilities.git
   cd docker-compose-utilities

2. Navigate to the folder of the service you want to use:
    cd cassandra-docker-compose

3. Follow the instructions in the individual folder's README.md to start the service.
    
## Contribution Guidelines
    We welcome contributions to improve and expand this repository. Please follow these guidelines:

    Reporting Issues
    - Use the Issues tab to report bugs or suggest new features.
    - Provide as much detail as possible, including steps to reproduce the issue.
    
    Submitting Changes
    1. Fork the repository and create a new branch for your changes:
        git checkout -b feature/your-feature-name
    2. Make your changes and test them thoroughly.
    3. Commit your changes with a descriptive message:
        git commit -m "Add support for XYZ service"
    4. Push your branch to your forked repository:
        git push origin feature/your-feature-name
    5. Open a pull request to the main repository. Include a detailed description of your changes.
    
    Code Style
    1. Follow the existing structure and naming conventions.
    2. Ensure your docker-compose.yml files are valid by running:
        docker-compose config

    Adding New Services
    1. Create a new folder named <service-name>-docker-compose/.
    2. Include a docker-compose.yml file and a README.md with setup instructions.
    3. Test your configuration before submitting a pull request.


Acknowledgments
Special thanks to the open-source community for providing the Docker images and tools used in this repository.
