# Delta Price Tracker

A Python application that monitors Delta Airlines flight prices and notifies users when prices drop, helping travelers save money through Delta's price difference refund policy.

## Features

- Monitor specific flight prices using Google Flights API
- Email notifications for price drops
- User dashboard for tracking multiple flights
- Price history tracking and analysis
- Configurable notification preferences

## Installation

### Prerequisites

- Python 3.8+
- pip

### Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/delta-price-tracker.git
cd delta-price-tracker
```

2. Create and activate virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Create `.env` file and add your configuration:
```bash
cp .env.example .env
# Edit .env with your settings
```

## Usage

Basic usage example:

```python
from delta_price_tracker import FlightTracker

tracker = FlightTracker()
tracker.add_flight("JFK", "LAX", "2024-02-01")
tracker.start_monitoring()
```

For more examples, see the [documentation](docs/index.rst).

## Development

### Setting up development environment

1. Install development dependencies:
```bash
pip install -r requirements-dev.txt
```

2. Install pre-commit hooks:
```bash
pre-commit install
```

### Running tests

```bash
pytest
```

### Code Style

This project uses:
- black for code formatting
- flake8 for style guide enforcement
- mypy for type checking
- isort for import sorting

## Documentation

Full documentation is available in the `docs` directory.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Google Flights API via RapidAPI
- [List any other tools/libraries you're using]

## Project Status

Under active development - MVP in progress.

## Contact

Your Name - your.email@example.com

Project Link: https://github.com/yourusername/delta-price-tracker