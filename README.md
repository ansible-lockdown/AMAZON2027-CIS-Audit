# AMAZON 2027 Syver config

## Overview

### Beta 0.0.1, based on CIS Amazon Linux 2023 Benchmark v2.0.0

**Beta: CIS has not yet published an Amazon Linux 2027 benchmark.** Until it does, this audit follows the control numbering and content of the CIS Amazon Linux 2023 Benchmark v2.0.0, adapted for Amazon Linux 2027. Use it for testing only. The audit will move to the official benchmark when CIS releases it.

[Centre For Internet Security]

This repository is set of configuration files and directories to run the audit of the relevant benchmark of Amazon Linux 2027 servers

This is configured in a directory structure level.

## variables

file: vars/{benchmark_type}.yml

Please refer to the file for all options and their meanings

The listed variable for every control/benchmark can be turned on/off or section

- Other controls
  - enable_selinux
  - run_heavy_tasks

- Bespoke options

  If a site has specific options e.g. password complexity these can also be set.

## Requirements

syver >= 0.16.0 - the continuation of goss, reading the same goss file format. Syver replaces goss as it is a signed fork that is regularly updated.
root privileges

## Branches

If running as part of the ansible playbook, this will pull in the relevant branch for the version of benchmark you are remediating.

- e.g. v2.0.0 will pull in branch benchmark-v2.0.0

Devel is normally the latest benchmark version, so maybe different from the version of benchmark you wish to test.
Details will show in the README as part of the remediation as to the benchmark for the version it is written for.

## Usage

Fot the latest information on audit and how it can be used please visit

[Read the Docs - Audit]

## Extra settings

Ability to add your own requirements is available in several sections

## Support

[Discord Community Discussions]

[Enterprise Support]

[MindPoint Group]

## Contributing

Bug reports and feature requests are welcome from everyone, please raise an issue.

Pull requests are accepted from approved contributors only. To be onboarded, join the [Discord Server](https://www.lockdownenterprise.com/discord) and request contributor access. See [CONTRIBUTING.rst](CONTRIBUTING.rst) for the full process.

## Links and Further information

- [Syver]
  - [Syver documentation]
  - [goss vs Syver]
- [Centre For Internet Security]

<!----
README Links
---->

[benchmark-type]: CIS
[OS-VERSION]: AMAZON2027
[os-type]: Linux
[Centre For Internet Security]: https://www.cisecurity.org
[Read the Docs - Audit]: https://ansible-lockdown.readthedocs.io/en/latest/audit/getting-started-audit.html

[Syver documentation]: https://github.com/krameff/syver/blob/main/docs/index.md

[goss vs Syver]: https://github.com/krameff/syver/blob/main/docs/goss-vs-syver.md

[Syver]: https://github.com/krameff/syver
- [CIS standards](https://www.cisecurity.org)

[MindPoint Group]: https://mindpointgroup.com/cybersecurity-consulting/automate/baseline-modernization#GH_LockdownReadMe
[Discord Community Discussions]: https://www.lockdownenterprise.com/discord
[Enterprise Support]: https://lockdownenterprise.com#GH_LockdownReadMe
