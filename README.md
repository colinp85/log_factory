# log_factory

This is a factory for setting up sensible defaults for the python logging module, including:

* configuration of format and default level
* ability to add a file handler with different log level
* helper to set the log level
* an ArgumentParser that can be inherited

## Usage

```python
import log_factory
import logging

log_factory.create()
log_factory.set_log_level(logging.DEBUG)
log_factory.add_file_handler('out.log')

logger = log_factory.get_logger('example')

logger.info('hello!')
```

## Installation

From PIP:

```bash
pip install log_factory
```

Or pulled from git master:

```bash
pip install git+https://github.com/colinp85/log_factory
```
