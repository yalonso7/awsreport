<p align="center">
  <h3 align="center">AWS Report</h3>
  <p align="center">AWS Report is a tool for analyzing amazon resources.</p>

  <p align="center">
    <a href="https://twitter.com/bsd0x1">
      <img src="https://img.shields.io/badge/twitter-@bsd0x1-blue.svg">
    </a>
    <a href="https://www.gnu.org/licenses/gpl-3.0">
      <img src="https://img.shields.io/badge/License-GPLv3-blue.svg">
    </a>
  </p>
</p>

<hr>

### Install using PIP

```
pip install awsreport
```

### Features

* Search IAM users based on creation date
* Search buckets public
* Search security based in rules, default is 0.0.0.0/0
* Search elastic ip dissociated
* Search volumes available
* Search AMIs with permission public
* Search internet gateways detached

### Options

```
aws_report.py [OPTIONS]

Options:
  --s3          Search buckets public in s3
  --iam         Search iam users based on creation date
  --iam-max-age Use max-age to search for users created more than X days ago
  --sg          Search security groups with inbound specific rule
  --elasticip   Search elastic IP not associated
  --volumes     Search volumes available
  --ami         Search AMIs with permission public
  --owner       Defines the owner of the resources to be found
  --igw         Search internet gateways detached
  --help        Show this message and exit.

Examples:
    python awsreport.py --s3
    python awsreport.py --iam --owner 296192063842
    python awsreport.py --iam --iam-max-age 60
    python awsreport.py --sg --cidr 192.168.1.0/24 or
    python awsreport.py --sg (cidr default is 0.0.0.0)
```

### Developer contact

```
[+] Twitter: @bsd0x1
[+] Telegram: @bsd0x
[+] Github: /bsd0x
```
