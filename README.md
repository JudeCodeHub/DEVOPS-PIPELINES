# DevOps Pipelines

A simple JavaScript project for learning and demonstrating CI/CD automation with GitHub Actions.

The repository includes a basic Node.js application, a test script, and an automated workflow that installs dependencies and runs tests whenever changes are pushed to the `main` branch.

## Features

- Basic JavaScript application
- Node.js project configuration
- Automated testing with npm scripts
- GitHub Actions CI pipeline
- Automatic execution on pushes to `main`
- Ubuntu-based CI runner
- Beginner-friendly DevOps structure

## Project Structure

```text
DEVOPS-PIPELINES/
├── .github/
│   └── workflows/
│       └── pipeline.yaml   # GitHub Actions CI workflow
├── index.js                # Main application entry point
├── test.js                 # Test execution script
├── package.json            # Project metadata and npm scripts
└── README.md               # Project documentation
```

## Technology Stack

- **Language:** JavaScript
- **Runtime:** Node.js
- **Automation:** GitHub Actions
- **CI Environment:** Ubuntu
- **Package Manager:** npm

## Getting Started

### Prerequisites

Install the following tools before running the project locally:

- Node.js 16 or later
- npm
- Git

### Clone the Repository

```bash
git clone https://github.com/JudeCodeHub/DEVOPS-PIPELINES.git
cd DEVOPS-PIPELINES
```

### Install Dependencies

```bash
npm install
```

This project currently has no external runtime dependencies, but installing packages ensures the project is prepared for future additions.

## Running the Application

Run the application with:

```bash
npm run run
```

This executes `index.js` and displays basic DevOps and CI/CD messages in the terminal.

You can also run the entry point directly:

```bash
node index.js
```

## Running Tests

Run the test script with:

```bash
npm test
```

The test command executes `test.js` and provides simple output that can be used to verify that the CI pipeline is working correctly.

You can also run the test file directly:

```bash
node test.js
```

## Continuous Integration

The GitHub Actions workflow is defined in:

```text
.github/workflows/pipeline.yaml
```

The CI pipeline runs automatically whenever code is pushed to the `main` branch.

### Pipeline Steps

1. Checks out the repository code.
2. Sets up Node.js 16.
3. Installs project dependencies.
4. Runs the test script.

The workflow uses an Ubuntu environment provided by GitHub Actions.

## Workflow Status

To view the latest pipeline results:

1. Open the repository on GitHub.
2. Select the **Actions** tab.
3. Choose the **CI pipeline** workflow.
4. Review the workflow run and test output.

## Development Workflow

A typical development process is:

```bash
git checkout -b feature/your-change
# Make changes
npm test
git add .
git commit -m "Describe your change"
git push origin feature/your-change
```  
## Author

Maintained by [JudeCodeHub](https://github.com/JudeCodeHub).
