# Supply Chain Management Platform

## Project Overview
This project is a Flask-based platform for managing and visualizing supply chains. It provides features such as:

- **Supply Chain Mapping**: Visualize supplier networks and dependencies.
- **Blockchain Tracking**: Simulate immutable transaction records for transparency.
- **Smart Contract Simulation**: Automate supplier selection based on bids.
- **Risk Management Dashboard**: Analyze risks and disruptions in the supply chain.
- **Real-Time Data Integration**: Fetch live supply chain data from Kaggle, Open Supply Hub, and Data.gov.

## Features
1. **Supply Chain Mapping**
   - Visualizes supplier tiers and dependencies using `networkx`.
2. **Blockchain-Based Tracking**
   - Implements a simple blockchain to simulate transaction flows.
3. **Smart Contract Simulation**
   - Automates supplier selection with dynamic bids.
4. **Risk Management Dashboard**
   - Highlights risks and disruptions using real or simulated data.
5. **Automated Deployment**
   - GitHub Actions for CI/CD to AWS Elastic Beanstalk.

## Tech Stack
- **Backend**: Flask
- **Visualization**: matplotlib, networkx
- **Blockchain**: Python custom implementation
- **Automation**: GitHub Actions
- **Cloud**: AWS Elastic Beanstalk

## Getting Started

### Prerequisites
- Python 3.9+
- AWS CLI and Elastic Beanstalk CLI (for deployment)
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/supply-chain-project.git
   cd supply-chain-project
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application locally:
   ```bash
   python application.py
   ```

4. Access the app in your browser at `http://127.0.0.1:5000`.

## Deployment

### Deploy Locally
1. Run the Flask app:
   ```bash
   python application.py
   ```

2. Access the app in your browser at `http://127.0.0.1:5000`.

### Deploy to AWS Elastic Beanstalk

1. Initialize Elastic Beanstalk:
   ```bash
   eb init
   ```
   - Select your application name.
   - Choose Python as the platform.
   - Set the region (e.g., `us-east-1`).

2. Create an environment:
   ```bash
   eb create supply-chain-env
   ```

3. Deploy the application:
   ```bash
   eb deploy
   ```

4. Access the application using the provided public URL.

### Automate Deployment
1. Ensure your GitHub repository contains a `.github/workflows/deploy.yml` file.
2. Push to the `main` branch, and GitHub Actions will deploy your app automatically.

## File Structure
```
.
├── application.py          # Main Flask application
├── requirements.txt        # Python dependencies
├── Procfile                # Deployment configuration for Elastic Beanstalk
├── .github/workflows       # CI/CD workflows
├── static/                 # Static assets (if any)
├── templates/              # HTML templates (if any)
```

## Contributing
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## License
This project is licensed under the MIT License. See `LICENSE` for details.

## Contact
For questions or suggestions, feel free to reach out:
- **Email**: kanase.vijay09@gmail.com
- 
