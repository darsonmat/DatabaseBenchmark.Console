# Database Benchmark for Console
## Overview
Database Benchmark for Console is a multi-platform console implementation of Database Benchmark (https://github.com/STSSoft/DatabaseBenchmark).

It provides the basic functionality needed to perform a database evaluation:

* Tests the different databases, acording to the methodology described here: https://github.com/STSSoft/DatabaseBenchmark.Core
* Generates reports with the test results in CSV or JSON format.

## Supported platforms
* Windows - requires Microsoft .NET Framework 4.0+ or Mono 4.0.0+
* Linux - requires Mono 4.0.0+

## Basic usage

* Starting the application. If no arguments are provided, the application searches for the default configuration file "DefaultConfig.config" in the application startup directory :
```Shell
DatabaseBenchmark.Console
```

* Create a default configuration file (if none available):
```Shell
DatabaseBenchmark.Console --createConfig="path_to_create_file"
```

* Start the benchmarking with a specified configuration file:
```Shell
DatabaseBenchmark.Console --configPath="path_to_config_file"
```

* Start the benchmarking and generate report at finish:
```Shell
DatabaseBenchmark.Console --configPath="path_to_config_file" --csvPath="path_to_CSV_file" --report=detailed
```


