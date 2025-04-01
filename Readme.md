# Logging in PySpark Application

## Overview  
This project demonstrates effective logging in a PySpark-based Python application, including custom log formatters, log file management, and error handling.  

## Features  

### Different Log Formatters  
Implemented two different log formats based on logging needs, capturing timestamps, function names, log levels, and file details.  

### Custom Log File  
Logs are stored in a dedicated log file with a timestamp-based filename for better tracking.  

### PySpark Initialization & Data Processing  
- PySpark session is initiated for data processing.  
- CSV file read operation is logged.  
- The total number of records is logged for transparency.  

### Error Handling in PySpark  
- A deliberate error (accessing a non-existent column) is introduced.  
- The error is caught and logged using `logger.error()` to help in debugging.  

### Logging Levels Used  
- `logger.info()` for key process updates.  
- `logger.error()` for exception handling with error messages.  

### Graceful Shutdown of Logging  
- Used `logging.shutdown()` to ensure all log messages are written to the file before exiting.  

### Log Storage Optimization  
- Ensured logs are efficiently written to a file instead of just printing to the console.  
- Configured logging handlers to manage log output efficiently.  
