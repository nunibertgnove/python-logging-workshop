# Python Logging Workshop

## Introduction
Logging is essential for building reliable and observable software. This repository contains a comprehensive guide to Python's built‑in `logging` module, covering fundamentals, configuration, and best practices.

## Why Logging Matters
- **Debugging**: Capture runtime details to reproduce and fix issues.
- **Monitoring**: Enable health checks and alerts by aggregating logs.
- **Auditing**: Keep records for compliance and forensics.
- **Performance Insight**: Track execution flow and identify bottlenecks.

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

For deeper coverage, see `WORKSHOP_GUIDE.md` and the research notes in `logging-research/logging-notes.md`.
