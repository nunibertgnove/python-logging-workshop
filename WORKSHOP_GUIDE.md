# Python Logging Workshop

## Introduction
Logging is a critical practice for building reliable, observable, and maintainable software. This workshop provides a comprehensive guide to Python's built‑in `logging` module, covering concepts, configuration, and real‑world patterns.

## Why Logging Matters
- **Debugging**: Capture detailed runtime information to reproduce and fix issues.
- **Monitoring**: Enable health checks and alerting by aggregating logs.
- **Auditing**: Maintain records of operations for compliance and forensic analysis.
- **Performance Insight**: Track execution flow and bottlenecks.

## Getting Started Guide
1. **Import and create a logger**
   ```python
   import logging
   logger = logging.getLogger(__name__)
   ```
2. **Configure the root logger** (simple scripts)
   ```python
   logging.basicConfig(level=logging.INFO, filename='app.log')
   ```
3. **Emit log messages**
   ```python
   logger.debug('Debug details')
   logger.info('Informational message')
   logger.warning('Potential issue')
   logger.error('Error occurred')
   logger.critical('Critical failure')
   ```
4. **Advanced configuration** – use `logging.config.dictConfig` or a YAML file to define multiple handlers, formatters, and log levels.

For deeper coverage, see the accompanying `logging-notes.md` in the `logging-research` folder.
