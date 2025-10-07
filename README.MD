# Field Engineering Tools Repository Template
This repo and organziation is not supported by Snowflake, use at your own risk. These are collections of scripts and automations that we use.

This repository serves as a central location for scripts and tools used by the Applied Field Engineering team. Please follow these guidelines when adding new scripts or modifying existing ones.

## Repository Structure

```
field-engineering-tools/
├── scripts/
│   ├── automation/        # Automation scripts for common tasks
│   ├── diagnostics/       # Diagnostic and troubleshooting tools
│   ├── deployment/        # Installation and deployment scripts
│   ├── monitoring/        # Monitoring and reporting tools
│   └── utilities/         # General utility scripts
├── docs/
│   ├── guides/            # User guides for scripts
│   └── templates/         # Documentation templates
├── tests/                 # Test files for the scripts
├── CONTRIBUTING.md        # Contribution guidelines
├── LICENSE                # License information
└── README.md              # Repository overview
```

## Script Template

When adding a new script, please use the following template structure:

```
#!/usr/bin/env [language interpreter e.g. python3, bash, etc.]

# -------------------------------------------------------
# Script Name: [Name of the script]
# Author: [Your Name]
# Creation Date: [YYYY-MM-DD]
# Last Modified: [YYYY-MM-DD]
# Version: [e.g. 1.0.0]
# 
# Description:
#   [Detailed description of what the script does]
#
# Usage:
#   [How to execute the script with example commands]
#
# Arguments:
#   [List and explain each argument]
#
# Requirements:
#   [List any dependencies or requirements]
#
# Example:
#   [Provide a complete example of how to use the script]
# -------------------------------------------------------

# Import statements and global variables

# Function definitions

# Main execution

# Error handling
```

## Documentation Requirements

Each script must include:

1. A detailed header as shown in the template above
2. Inline comments for complex logic
3. A corresponding entry in the README.md file
4. (Optional but recommended) A more detailed guide in the docs/guides/ directory

## Best Practices

1. **Naming Convention**: Use descriptive names with underscores (e.g., `deploy_app_to_production.sh`, `diagnose_network_issue.py`)
2. **Modular Design**: Write modular code with reusable functions
3. **Error Handling**: Include robust error handling and meaningful error messages
4. **Logging**: Implement appropriate logging for troubleshooting
5. **Parameter Validation**: Validate input parameters before execution
6. **Exit Codes**: Use meaningful exit codes to indicate success/failure

## Testing

1. Each script should have basic test coverage
2. Place tests in the corresponding directory under the `tests/` folder
3. Tests should verify that the script works as expected with various inputs

## Contribution Process

1. Create a branch with a descriptive name (e.g., `add-network-diagnostics-script`)
2. Develop and test your script locally
3. Submit a pull request with a detailed description
4. Ensure your script follows the template and best practices
5. Address any feedback from code reviewers

## Version Control

1. Use semantic versioning for scripts (MAJOR.MINOR.PATCH)
2. Update the "Last Modified" date in the script header when changes are made
3. Document significant changes in a changelog section or separate CHANGELOG.md file

## Security Considerations

1. Never include credentials or sensitive data in scripts
2. Use environment variables or secure credential storage
3. Validate and sanitize all inputs to prevent injection attacks
4. Apply the principle of least privilege when scripting system operations

## README Template for New Scripts

When adding a new script, update the main README.md file with an entry like this:

```markdown
### [Script Name]

**Location**: scripts/[category]/[script_name]
**Purpose**: [Brief description]
**Author**: [Your Name]
**Added**: [YYYY-MM-DD]

[One or two sentences about when/how to use this script]

Example usage:
```bash
./scripts/[category]/[script_name] [example arguments]
```
```

## License

All contributions to this repository will be under the [repository's license]. Please make sure you understand and agree to these terms before contributing.
