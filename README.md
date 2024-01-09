# Two-Factor Authentication Example

This project provides a simple implementation of two-factor authentication (2FA) using Node.js, Express, and the speakeasy library.

## Getting Started

### Prerequisites

Make sure you have the following installed on your machine:

- Node.js (https://nodejs.org/)
- npm (Node Package Manager)

### Installation

1. Clone the repository:
    git clone https://github.com/your-username/two-factor-authentication-example.git


Navigate to the project directory:
    
    cd two-factor-authentication-example

Install dependencies:

    npm install

## Usage

1. Start the server:

    npm start

2. Access the API at http://localhost:5000/api.

## API Endpoints
1. Welcome

    Endpoint: `GET /api`
    Description: Welcome message for the two-factor authentication example.

2. Register User

    Endpoint: `POST /api/register`
    Description: Register a user and generate a temporary secret for 2FA.

3. Verify Token

    Endpoint: `POST /api/verify`
    Description: Verify the generated token for a registered user.

4. Validate Token

    Endpoint: `POST /api/validate`
    Description: Validate a token for a user with an established 2FA secret.

## Example Requests
### Register User

    curl -X POST http://localhost:5000/api/register

### Verify Token

    curl -X POST -H "Content-Type: application/json" -d '{"userId": "user-id", "token": "123456"}' http://localhost:5000/api/verify

### Validate Token

    curl -X POST -H "Content-Type: application/json" -d '{"userId": "user-id", "token": "123456"}' http://localhost:5000/api/validate

## Contributing

Contributions are welcome! Feel free to open issues or pull requests.

## License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.