# HDFS Data Analysis Report

## Overview
This report provides an analysis of parsed HDFS log data, including the distribution of normal and anomalous lines, event types, sequences, and count vectors.

## Summary Statistics

### Parsed Lines
- **Total Parsed Lines:** 12,580,989
- **Normal Lines:** 12,255,230 (97.4%)
- **Anomalous Lines:** 325,759 (2.6%)

### Event Types
- **Total Event Types:** 33
- **Normal Event Types:** 20 (60.6%)
- **Anomalous Event Types:** 32 (97.0%)

### Sequences
- **Total Sequences:** 575,061
- **Normal Sequences:** 558,223 (97.1%)
- **Anomalous Sequences:** 16,838 (2.9%)
- **Unique Sequences:** 26,814 (4.7%)
- **Unique Normal Sequences:** 21,690 (80.9%)
- **Unique Anomalous Sequences:** 5,133 (19.1%)
- **Sequences Labeled Normal That Also Occur as Anomalous:** 14 (0.003%), 9 unique
- **Sequences Labeled Anomalous That Also Occur as Normal:** 17 (0.101%), 9 unique

## Common Sequences

### Common Normal Sequences
1. **73,691 occurrences** - ('5', '5', '5', '22', '11', '9', '11', '9', '11', '9', '26', '26', '26', '23', '23', '23', '30', '30', '30', '21', '21', '21')
2. **40,156 occurrences** - ('5', '22', '5', '5', '11', '9', '11', '9', '11', '9', '26', '26', '26', '23', '23', '23', '30', '30', '30', '21', '21', '21')
3. **37,788 occurrences** - ('5', '5', '22', '5', '11', '9', '11', '9', '11', '9', '26', '26', '26', '23', '23', '23', '30', '30', '30', '21', '21', '21')

### Common Anomalous Sequences
1. **1,643 occurrences** - ('5', '22')
2. **1,361 occurrences** - ('22', '5', '5', '7')
3. **1,307 occurrences** - ('22', '5')

## Unique Count Vectors
- **Total Unique Count Vectors:** 666 (2.5% of unique sequences or 0.1% of all sequences)
- **Normal Count Vectors:** 257 (38.6%)
- **Anomalous Count Vectors:** 418 (62.8%)
- **Count Vectors Labeled Normal That Also Occur as Anomalous:** 230 (0.041%), 9 unique
- **Count Vectors Labeled Anomalous That Also Occur as Normal:** 316 (1.877%), 9 unique

### Common Normal Count Vectors
1. **300,011 occurrences** - (('11', 3), ('21', 3), ('22', 1), ('23', 3), ('26', 3), ('30', 3), ('5', 3), ('9', 3))
2. **96,316 occurrences** - (('11', 3), ('22', 1), ('26', 3), ('5', 3), ('9', 3))
3. **21,127 occurrences** - (('11', 3), ('21', 3), ('22', 1), ('23', 3), ('26', 3), ('3', 1), ('30', 3), ('4', 2), ('5', 3), ('9', 3))

### Common Anomalous Count Vectors
1. **3,225 occurrences** - (('22', 1), ('5', 2), ('7', 1))
2. **3,182 occurrences** - (('11', 3), ('20', 1), ('21', 3), ('22', 1), ('23', 3), ('26', 3), ('30', 3), ('5', 3), ('9', 3))
3. **2,950 occurrences** - (('22', 1), ('5', 1))

## Conclusion
This analysis provides insights into the distribution of normal and anomalous sequences in the HDFS logs. While most sequences and count vectors are normal, anomalous sequences exhibit distinct patterns that can be leveraged for anomaly detection and system monitoring.

