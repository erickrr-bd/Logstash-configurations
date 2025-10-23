# Logstash-configurations

Modular collection of custom configurations and filters for Logstash, designed to adapt log parsing to particular structures of enterprise systems and applications. 

# Features
- Modular filters by system/application
- Compatibility with ECS and business pipelines
- Robust parsing for ambiguous delimiters and mixed structures
- Validation of key fields for traceability and auditing

# Configurations
- RHEL 8/CentOS 8/Rocky Linux 8 (auditd/audisp)
- RHEL 7/CentOS 7/Rocky Linux 7 ([uAuditAnalyzer](https://github.com/unmanarc/uAuditAnalyzer2))
- Firewall (FW-5600)
- Kaspersky
- Deep Security Manager
- F5 BIG-IP (WAF)
- AIX System

# Requirements
- Logstash version 7.x or 8.x

# Usage

Copy the filter to your Logstash pipeline or configuration.

# Recommendations
- Validate filters with real data before production
- Document exclusions and unmapped fields
- Alinear los pipelines a controles de auditoría y continuidad operativa

# Contributions

Improvements, new filters and additional documentation are accepted. 
