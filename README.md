# 🚀 Logstash Configurations

A modular collection of custom configurations and advanced filters for Logstash. This repository is designed to bridge the gap between complex enterprise log structures and actionable data, ensuring compatibility with the Elastic Common Schema (ECS).

## ✨ Key Features
- Modular Architecture: Independent filters organized by system and application.
- Enterprise Ready: Robust parsing for ambiguous delimiters and mixed structures.
- Compliance Focused: Validation of key fields to support traceability, auditing, and forensic analysis.
- ECS Aligned: Designed to maintain consistency across business pipelines and dashboards.

## 📂 Supported Configurations
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

## 🛠️ Requirements
- Logstash Engine: Versions 7.x or 8.x.
- Plugins: Ensure logstash-filter-grok, logstash-filter-mutate, and logstash-filter-date are installed (standard in most distributions).

## 🚀 Usage & Deployment

1. Clone the repository:

`https://github.com/erickrr-bd/Logstash-configurations.git`

2. Integrate Filters: Copy the desired .conf file from the filters/ directory to your Logstash pipeline path:

`cp ./filters/nsx.conf /etc/logstash/conf.d/`

3. Test Configuration: Always validate your syntax before restarting the service:

`/usr/share/logstash/bin/logstash -f /etc/logstash/conf.d/nsx.conf --config.test_and_exit`

## 💡 Best Practices & Recommendations

[!IMPORTANT]
Data Privacy: Ensure that sensitive information (PII) is masked or dropped during the filter stage before reaching the index.

- Testing: Validate filters with a sample of real production data in a staging environment.
- Documentation: Maintain a record of exclusions and any unmapped fields specific to your organization.
- Compliance: Align your pipeline logic with internal audit controls and operational continuity standards.

## 🤝 Contributions

Contributions are welcome! If you have a new filter or performance improvement:

- Make a Fork of the project.
- Create a Branch for your improvement (`git checkout -b feature/AmazingFilter`).
- Commit your changes.
- Open a Pull Request.
