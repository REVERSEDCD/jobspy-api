# JobSpy API 🚀

![JobSpy API](https://img.shields.io/badge/JobSpy_API-Dockerized-brightgreen)

Welcome to the **JobSpy API** repository! This project provides a Dockerized version of the JobSpy job search utility. It features API key authentication, rate limiting, and proxy support to enhance your job search experience. 

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Dockerized Environment**: Run the application easily with Docker.
- **API Key Authentication**: Secure your API access with key-based authentication.
- **Rate Limiting**: Control the number of requests to avoid overloading.
- **Proxy Support**: Use proxies for scraping job listings from various platforms.
- **Multi-Platform Support**: Integrates with Glassdoor, Google Jobs, LinkedIn, and more.

## Technologies Used

- **Docker**: For containerization.
- **FastAPI**: A modern web framework for building APIs.
- **Python**: The programming language used for development.
- **Job Scraping Libraries**: Tools for extracting job listings.

## Installation

To get started with the JobSpy API, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/REVERSEDCD/jobspy-api.git
   cd jobspy-api
   ```

2. **Build the Docker Image**:
   ```bash
   docker build -t jobspy-api .
   ```

3. **Run the Docker Container**:
   ```bash
   docker run -d -p 8000:8000 jobspy-api
   ```

4. **Download the Latest Release**:  
   Visit [Releases](https://github.com/REVERSEDCD/jobspy-api/releases) to download the latest version. Execute the downloaded file to start using the API.

## Usage

Once the API is running, you can access it at `http://localhost:8000`. 

### Example Request

To get job listings, send a GET request to:

```
GET /jobs
```

Make sure to include your API key in the request headers.

### Sample Curl Command

```bash
curl -X GET "http://localhost:8000/jobs" -H "Authorization: Bearer YOUR_API_KEY"
```

## API Documentation

The API provides several endpoints for job searching. Here are a few key ones:

- **GET /jobs**: Retrieve job listings.
- **POST /jobs**: Create a new job listing (if applicable).
- **GET /jobs/{id}**: Retrieve details of a specific job listing.
- **DELETE /jobs/{id}**: Remove a job listing.

For more details, check the API documentation available in the repository.

## Contributing

We welcome contributions! If you want to help improve JobSpy API, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/YourFeature`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/YourFeature`.
5. Open a Pull Request.

Please ensure your code adheres to the coding standards of the project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, feel free to reach out:

- **Email**: support@jobspy.com
- **Twitter**: [@JobSpyAPI](https://twitter.com/JobSpyAPI)

---

Thank you for your interest in JobSpy API! We hope you find it useful for your job search needs. For updates and releases, visit [Releases](https://github.com/REVERSEDCD/jobspy-api/releases).