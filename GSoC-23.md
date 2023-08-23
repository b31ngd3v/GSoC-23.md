![GSoC 2023](https://developers.google.com/open-source/gsoc/resources/downloads/GSoC-logo-horizontal-800.png)

# Google Summer of Code'23 Final Report

- **Name**: Pramurta Sinha ([@b31ngd3v](https://github.com/b31ngd3v))
- **Organization**: [Python Software Foundation](https://www.python.org/psf/)
- **Sub-organization**: [CVE Binary Tool](https://github.com/intel/cve-bin-tool)
- **Project**: [Add GitHub Action including fancy reporting and triage integration](https://summerofcode.withgoogle.com/programs/2023/projects/rfhFsBbN)
- **Proposal**: [View/Download](https://blogs.python-gsoc.org/media/proposals/gsoc-proposal.pdf)

---

## Summary

### CVE Binary Tool Basic GitHub Action

Developed a github action for cve-bin-tool which will produce CVE reports in the GitHub security tab and will be able to split the issues on the basis of triage. It will be smart enough to scan dependency lists of various languages and suggest version upgrades. Also it will produce reports in the form of html and pdf by default in the security tab.

### SBOM Integration

Added the feature which will help the tool running as a GitHub Action to detect and scan SBOM files in the repository and will help to generate an SBOM and keep it up to date through regular scans.

### Mirror Work

CVE Binary Tool uses NVD's vulnerability database, there is a lot of restrictions like rate limiting even when using an API key. So I and [John](https://github.com/warthog9) created a mirror that will host the NVD data and made the tool compatible to use the mirror data.

## Tasks Achieved

#### - **Basic GitHub Action**:

**PRs**:

- [intel/cve-bin-tool-action#1](https://github.com/intel/cve-bin-tool-action/pull/1)
- [intel/cve-bin-tool-action#4](https://github.com/intel/cve-bin-tool-action/pull/4)
- [intel/cve-bin-tool-action#6](https://github.com/intel/cve-bin-tool-action/pull/6)
- [intel/cve-bin-tool-action#7](https://github.com/intel/cve-bin-tool-action/pull/7)
- [intel/cve-bin-tool-action#10](https://github.com/intel/cve-bin-tool-action/pull/10)
- [intel/cve-bin-tool-action#14](https://github.com/intel/cve-bin-tool-action/pull/14)
- [intel/cve-bin-tool-action#15](https://github.com/intel/cve-bin-tool-action/pull/15)
- [intel/cve-bin-tool-action#16](https://github.com/intel/cve-bin-tool-action/pull/16)
- [intel/cve-bin-tool-action#22](https://github.com/intel/cve-bin-tool-action/pull/22)
- [intel/cve-bin-tool-action#23](https://github.com/intel/cve-bin-tool-action/pull/23)
- [intel/cve-bin-tool-action#24](https://github.com/intel/cve-bin-tool-action/pull/24)

#### - **SBOM Integration**:

**PRs**:

- [intel/cve-bin-tool-action#25](https://github.com/intel/cve-bin-tool-action/pull/25)
- [intel/cve-bin-tool-action#26](https://github.com/intel/cve-bin-tool-action/pull/26)
- [intel/cve-bin-tool-action#30](https://github.com/intel/cve-bin-tool-action/pull/30)
- [intel/cve-bin-tool-action#31](https://github.com/intel/cve-bin-tool-action/pull/31)
- [intel/cve-bin-tool-action#32](https://github.com/intel/cve-bin-tool-action/pull/32)
- [intel/cve-bin-tool-action#37](https://github.com/intel/cve-bin-tool-action/pull/37)

## Future

I plan on contributing significantly to the project after the GSoC period. Things I plan to do:

- Improve the mirror system so that it can generate and export json files with the help of NVD API v2.
- Suporrting more versions of cyclonedx.

---

I am thankful to **Google**, **Python Software Foundation**, and **Intel** for providing me with this excellent opportunity and the mentors, [Terri Oda](https://github.com/terriko), [Anthony Harrison](https://github.com/anthonyharrison), [Anant](https://github.com/XDRAGON2002), and [Rhythm](https://github.com/rhythmrx9) who guided me throughout the program.

I would also like to thank my fellow GSoC contributor [Sukhveer](https://github.com/Rexbeast2) and the cve-bin-tool community for helping me during the program.
