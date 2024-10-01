# Flow Log Parser

## Overview
This program parses AWS-style flow log data and assigns tags based on a lookup table. The goal is to generate counts of matched tags and port/protocol combinations. 

## Assumptions
- Only default flow log formats (version 2) are supported.
- The log format and lookup table are expected to be in plain ASCII text.
- Case-insensitive matching for protocols is applied (e.g., `tcp`, `TCP`).
- The program is expected to handle up to 10 MB of flow log data.
- The lookup table can have up to 10,000 mappings.

## Instructions to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/rameshb8/flow-log-parser.git
   cd flow-log-parser
