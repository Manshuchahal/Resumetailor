# ResumeTailor

ResumeTailor is a web application that helps users create and tailor resumes according to a company's **Job Description (JD)**. Users can enter their information manually or upload an existing resume and use AI-powered analysis to improve the relevance of their resume for a specific job.

## Features

*  Upload an existing resume
*  Enter resume information manually
*  Tailor resumes according to a Job Description
*  AI-powered resume analysis
*  Identify relevant skills and keywords from a JD
*  Generate improved resume content
*  Multiple resume templates
*  Responsive web interface
*  Environment variables for API keys and sensitive configuration

## How It Works

1. Upload an existing resume or enter your details manually.
2. Paste the target company's Job Description.
3. ResumeTailor analyzes the JD and identifies important:

   * Skills
   * Keywords
   * Qualifications
   * Responsibilities
4. The application compares the resume with the JD.
5. AI generates tailored resume content based on the job requirements.
6. Select a resume template and generate the final resume.

## Tech Stack

### Frontend

* React
* JavaScript
* HTML
* CSS

### Backend

* Node.js
* Express.js
* REST API

### AI

* Google Gemini API

### Development Tools

* Git
* GitHub
* npm

## Project Structure

```text
resumetailor/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── ...
│   ├── .env
│   └── package.json
│
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

> The `.env` file contains sensitive credentials and is intentionally excluded from GitHub using `.gitignore`.

## Installation

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd resumetailor
```

### 2. Install Dependencies

Install the root dependencies:

```bash
npm install
```

Then install frontend and backend dependencies if they have separate `package.json` files:

```bash
cd frontend
npm install
```

```bash
cd ../backend
npm install
```

### 3. Configure Environment Variables

Create a `.env` file inside the `backend` directory:

```env
GEMINI_API_KEY=your_api_key_here
```

Add any other environment variables required by the backend.

**Never commit your `.env` file to GitHub.**

## Running the Application

Start the backend:

```bash
cd backend
npm start
```

Start the frontend in another terminal:

```bash
cd frontend
npm run dev
```

The frontend will normally be available at:

```text
http://localhost:5173
```

The backend will normally run on its configured port.

## Environment Variables

The backend may require the following variables:

| Variable         | Description                            |
| ---------------- | -------------------------------------- |
| `GEMINI_API_KEY` | Google Gemini API key                  |
| `PORT`           | Backend server port                    |
| `DATABASE_URL`   | Database connection URL, if applicable |

Do not publish real API keys, database credentials, JWT secrets, or other sensitive values.

## Deployment

The frontend and backend can be deployed separately.

### Frontend

The frontend can be deployed using services such as Netlify or Vercel.

### Backend

The backend can be deployed using a backend hosting provider that supports the application's runtime.

After deployment, update the frontend API URL so that it points to the production backend instead of `localhost`.

## Future Improvements

* ATS compatibility scoring
* Resume keyword matching
* More professional resume templates
* PDF export
* User authentication
* Resume version history
* Job-specific resume recommendations
* LinkedIn profile integration
* Job application tracking

## Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes.
5. Push the branch.
6. Create a Pull Request.

## License

This project is currently intended for educational and development purposes.
