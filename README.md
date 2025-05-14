# DevLedger

DevLedger is an intelligent knowledge persistence system that transforms code comments into a queryable, evolving knowledge graph across hardware and firmware domains through pattern-based tracking and LLM-powered analysis.

## Features

- **Pattern-based Comment Tracking**: Maintain comment identity through code changes
- **Multi-level Comment Organization**: Information, Debug, and Technical comment levels
- **Git Integration**: Seamless integration with Git workflow through hooks
- **LLM-powered Analysis**: Intelligent processing of comments and queries
- **Hardware-Software Bridge**: Connect knowledge across domains
- **Local-first Architecture**: Support for both local and cloud LLM deployments
- **Extensible Design**: Plugin architecture for custom functionality

## Installation

### Prerequisites
- Python 3.8+
- Git 2.25+
- 8GB+ RAM (recommended for local models)

### Basic Installation
```bash
pip install devledger
```

### Development Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/devledger.git
cd devledger

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install with development dependencies
pip install -e ".[dev]"
```

### Optional Components
```bash
# Install with all optional features
pip install "devledger[all]"

# Install specific features
pip install "devledger[vector]"  # For vector storage
pip install "devledger[local]"   # For local LLM support
pip install "devledger[cloud]"   # For cloud LLM support
```

## Basic Usage

### Initialize DevLedger in Your Repository
```bash
cd your-project
devl init
```

### Add Comments with DevLedger Patterns
```python
# I5- Basic initialization routine for the sensor module
def initialize_sensor():
    # D5- Calibration constant compensates for sensor nonlinearity
    TEMP_CALIBRATION = 1.024f
    ...
```

### Query Knowledge Base
```bash
# Understanding implementation decisions
devl why use_polling_for_sensor_reads

# Exploring hardware-software relationships
devl what connects to GPIO_PIN_5

# Discovering historical context
devl history temperature_calibration_value
```

### Generate Documentation
```bash
# Generate interface documentation
devl doc sensor_interface

# Create onboarding guide
devl guide power_management_subsystem
```

## Development Setup

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed development setup instructions.

### Quick Start for Development
1. Clone the repository
2. Create and activate a virtual environment
3. Install development dependencies
4. Install pre-commit hooks
5. Run tests to verify setup

## Documentation

- [Project Documentation](https://devledger.readthedocs.io/)
- [API Reference](https://devledger.readthedocs.io/en/latest/api/)
- [Contributing Guide](CONTRIBUTING.md)
- [Security Policy](SECURITY.md)

## Architecture

DevLedger employs a layered architecture:

1. **Knowledge Capture Layer**
   - Pattern-based comment tracking
   - Git hook integration
   - Multi-language support

2. **Storage Layer**
   - `.devl` directory structure
   - JSON/YAML storage format
   - Vector database integration

3. **Intelligence Layer**
   - LLM processing pipeline
   - Pattern recognition
   - Context analysis

4. **Interaction Layer**
   - CLI interface
   - Direct file editing
   - Query processing

## Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details on:
- Setting up your development environment
- Our coding standards
- The pull request process

## Security

For security concerns, please review our [Security Policy](SECURITY.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.