## Asynchronous Data Processing with Redash, OpenAI, and Celery

This project serves as a tutorial for implementing asynchronous data processing techniques in the context of Redash dashboards, utilizing OpenAI's API for natural language processing, and managing background tasks with Celery.

## Project Structure

````

## Getting Started

### Prerequisites
- Python 3.6 or higher
- Redis server
- Docker (optional, for running Redis)
- Jupyter Notebook or JupyterLab

### Setup and Installation

1. **Clone the Repository**
   ```sh
   git clone https://github.com/[your-username]/asynchronous-data-processing.git
   cd asynchronous-data-processing
````

2. **Create a Virtual Environment and Install Dependencies**

   ```sh
   python -m venv venv
   source venv/bin/activate  # For Unix or MacOS
   venv\Scripts\activate     # For Windows
   pip install -r requirements.txt
   ```

3. **Environment Variables**

   - Create a `.env` file in the root directory.
   - Add the following environment variable:
     ```
     OPENAI_API_KEY=your_openai_api_key
     ```

4. **Running Redis Using Docker**

   - If you have Docker installed, run the following command to start a Redis server:
     ```sh
     docker run --name my-redis -p 6379:6379 -d redis
     ```
   - This command downloads the Redis image and starts a Redis container.

5. **Running the Celery Worker**

   - In a new terminal, activate the virtual environment and run the Celery worker:
     ```sh
     celery -A celery_app worker --loglevel=info
     ```

6. **Launching the Jupyter Notebook**
   - In your virtual environment, start Jupyter Notebook or JupyterLab:
     ```sh
     jupyter notebook
     ```
   - Open `tutorial.ipynb` and run through the cells to understand the asynchronous data processing concepts.

## Contributing

Contributions, issues, and feature requests are welcome.

## Contact

Elias Andualem - eandualem@gmail.com(mailto:eandualem@gmail.com)

Project Link: https://github.com/eandulem/asynchronous-data-processing
