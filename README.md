# LMS Frontend

This is the frontend application for the Learning Management System (LMS). It is built using React and communicates with the backend API.

## Prerequisites

Before you begin, ensure you have the following installed on your system:
- [Node.js](https://nodejs.org/) (version 16 or higher)
- [npm](https://www.npmjs.com/) (comes with Node.js)
- [Docker](https://www.docker.com/) (optional, for containerized deployment)

## Getting Started

Follow these steps to set up and run the application locally:

### 1. Clone the Repository

```bash
git clone <repository-url>
cd LMS/client
```

### 2. Install Dependencies

Run the following command to install the required dependencies:

```bash
npm install
```

### 3. Configure Environment Variables

Ensure the `.env` file is correctly set up. By default, it should look like this:

```
REACT_APP_API_URL=http://localhost:5000/api
```

Update the `REACT_APP_API_URL` if your backend API is hosted on a different URL.

### 4. Run the Application

Start the development server:

```bash
npm start
```

The application will be available at `http://localhost:3000`.

### 5. Build for Production

To create a production build, run:

```bash
npm run build
```

The build files will be generated in the `build` directory.

## Docker Deployment

To run the application using Docker:

1. Build the Docker image:

   ```bash
   docker build -t lms-client .
   ```

2. Run the Docker container:

   ```bash
   docker run -p 80:80 lms-client
   ```

The application will be available at `http://localhost`.

## Project Structure

- `src/`: Contains the source code for the application.
- `public/`: Contains static assets.
- `.env`: Environment variables for the application.

## Useful Scripts

- `npm start`: Starts the development server.
- `npm run build`: Builds the application for production.
- `npm test`: Runs the test suite.

## Troubleshooting

If you encounter any issues, ensure that:
- The backend API is running and accessible.
- The `.env` file is correctly configured.
- All dependencies are installed (`npm install`).

For further assistance, contact the project maintainer.

