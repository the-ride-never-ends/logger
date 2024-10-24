# Logger Module

## Overview
The module sets up logging based on a configuration file (config.yaml) or falls back to default settings.
It supports various log levels (DEBUG, INFO, WARNING, ERROR, CRITICAL) and provides methods to log
messages with different severities. The Logger class can be instantiated with custom names, batch IDs,
and log levels, making it flexible for different parts of an application.

Includes:
1. A Logger class that creates loggers with dynamic log folder generation and routing capabilities.
2. A specialized prompt logger for use within LLM engines.
3. Utility functions for managing log files and generating unique IDs.
4. Configuration handling for log levels and global settings.


## Key Features
- Dynamic log file and folder creation
- Configurable log levels
- Special handling for prompt logging in LLM contexts
- Automatic formatting of log messages
- Support for both file and console logging

Usage:
    from logger import Logger
    logger = Logger(logger_name="my_app")
    logger.info("Application started")
    logger.debug("Debug information")
    logger.error("An error occurred")

Note: This module requires the 'yaml' package for configuration file parsing.

## Overview
This module provides functionality for managing configuration settings in Python applications. 
It offers a flexible and easy-to-use approach to handling configuration data, supporting both local files and environment variables.

## Key Features
- Load configuration from YAML files
- Support for environment variable overrides
- Nested configuration structure
- Easy access to configuration values
- Default value support

## Dependencies
This module requires the following external libraries:
- PyYAML

## Usage
To use this module, import it as follows:
```python
from logger import Logger
logger = Logger(logger_name="my_app")

logger.info("Application started")
logger.debug("Debug information")
logger.error("An error occurred")
