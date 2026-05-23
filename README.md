# Logstash-configurations

Modular collection of custom configurations and filters for Logstash, designed to adapt log parsing to particular structures of enterprise systems and applications. 

## Features
- Modular filters by system/application
- Compatibility with ECS and business pipelines
- Robust parsing for ambiguous delimiters and mixed structures
- Validation of key fields for traceability and auditing

## Configurations
- RHEL 8/Rocky Linux 8 (auditd/audisp) (Compatible with version 9)
- RHEL 7/Rocky Linux 7 ([uAuditAnalyzer](https://github.com/unmanarc/uAuditAnalyzer2))
- AIX System
- Imperva SecureSphere (DBF)
- BIG-IP F5 (WAF)
- Check Point FW-5600 (Firewall)
- Check Point SmartDefense
- GitHub Enterprise
- Kaspersky Security Center
- Deep Security Agent (Trend Micro)
- Trend Vision One (Trend Micro)
- Nutanix
- VMware NSX

## Requirements
- Logstash version 7.x or 8.x

## Usage

Copy the filter to your Logstash pipeline or configuration.

## Recommendations
- Validate filters with real data before production
- Document exclusions and unmapped fields
- Align pipelines to audit and operational continuity controls

## Contributions

Improvements, new filters and additional documentation are accepted. 
