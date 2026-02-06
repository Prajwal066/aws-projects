# Image Labels Generator – Amazon Rekognition

This project demonstrates how Amazon Rekognition can be used to analyze
images stored in Amazon S3 and automatically detect objects and labels.
The project is designed to apply AWS Cloud Practitioner (CLF-C02)
concepts using managed AI services.

---

## Overview

An image is uploaded to an Amazon S3 bucket. Amazon Rekognition analyzes
the image using the DetectLabels API and returns a list of detected labels
along with confidence scores.

The analysis is performed using the AWS CLI, which represents a real
production-style interaction with AWS services.

---

## AWS Services Used

- Amazon S3 – Object storage for images
- Amazon Rekognition – Image analysis and label detection
- AWS IAM – Access control (implicitly used by AWS CLI)

---

## Architecture

![Architecture](architecture/architecture.png)

**Flow:**
1. User uploads an image to Amazon S3
2. Amazon Rekognition reads the image from S3
3. Rekognition detects labels and confidence scores
4. Results are returned to the user via the CLI

---

## Example Output

- Architecture (100%)
- Building (100%)
- City (100%)
- Urban (100%)

---

## AWS Cloud Practitioner Concepts Demonstrated

- Managed AI services
- Region-specific service availability
- Object storage (S3)
- Service integration
- Shared Responsibility Model
- Cost-aware cloud usage

---

## Project Structure
image-labels-generator/
├── README.md
├── architecture/
│ └── architecture.png
├── screenshots/
│ ├── s3-upload.png
│ ├── rekognition-cli-command.png
│ └── rekognition-cli-output.png
└── learnings.md
