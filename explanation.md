# Project Structure Explanation

## Root Structure

```
├── README.md
└── Chatbot-UI/
```

## Main Application (Chatbot-UI/)

```
├── components/       # React components
├── pages/           # Next.js pages
├── public/          # Static assets
├── styles/          # CSS styles
├── types/           # TypeScript type definitions
├── utils/          # Utility functions
├── __tests__/      # Test files
```

## Infrastructure & Deployment

```
├── EKS-TF/         # Terraform files for EKS setup
│   ├── backend.tf   # S3 backend configuration
│   └── variables.tfvars  # Terraform variables
├── JenkinsFile/    # Jenkins pipeline definitions
│   ├── Chatbot-Jenkinsfile  # Main application pipeline
│   └── EKS-Jenkinsfile      # EKS deployment pipeline
├── k8s/            # Kubernetes manifests
├── Dockerfile      # Container definition
└── docker-compose.yml
```

## Configuration Files

```
├── next.config.js
├── next-i18next.config.js
├── tailwind.config.js
├── tsconfig.json
├── prettier.config.js
├── postcss.config.js
└── vitest.config.ts
```

## Build & Development

```
├── package.json
└── Makefile        # Build and run commands
```

## Key Components

- The application is a Next.js-based chatbot UI with TypeScript and Tailwind CSS
- Infrastructure is managed through Terraform (EKS-TF/)
- CI/CD is handled by Jenkins (JenkinsFile/)
- Containerization using Docker
- Kubernetes deployment configuration (k8s/)
- AWS EKS as the deployment platform
- S3 backend for Terraform state management
