# iOS/iPadOS 17.0 Hardening

Welcome to iOS/iPadOS 17.0 Hardening – your go-to repository for enhancing the security of iOS and iPadOS 17.0 devices managed through Microsoft Intune.

## About This Repository
<img align="right" src="https://rietveld-ict.nl/wp-content/uploads/2023/12/shield_small.png"/>

This repository contains JSON and custom .mobileconfig files designed to improve iOS/iPadOS 17.0 security via Microsoft Intune. The configuration settings are based on the baselines provided by CIS, following the industry-recognized [CIS Benchmarks](https://www.cisecurity.org/benchmark/apple_ios) for iOS/iPadOS 17.0 hardening. There are CIS Level 1 and Level 2 configuration files available. There is a difference in configuration between End-User owned devices and institutionally owned devices.

### End-user owned vs institutionally
In summary, the key differences between end-user owned and institutionally owned devices in the context of Apple iOS/iPadOS 17.0 management are:
* Supervision: Institutionally owned devices are often set to a "supervised" state, allowing for greater organizational control, unlike end-user owned devices which are typically unsupervised.
* Device Enrollment Program (DEP): Institutionally owned devices are typically enrolled in Apple's DEP, linking them directly to an organization's MDM server from activation, ensuring managed control from the outset.
* Management at Activation: Devices under DEP receive configuration and management settings as soon as they are activated, beneficial for new or factory-reset devices.
* Volume Purchase Program (VPP): This program is used for managing app licenses on institutionally owned devices, allowing organizations to maintain control over app distribution and licensing, a feature not commonly used for end-user owned devices.

It's important to note that the settings catalog in Intune does not cover all the security controls required by the CIS benchmark for iOS/iPadOS 17.0 17. To address this gap, you'll need to import the .mobileconfig files using the "Profile Templates > Custom" option in Intune. These additional files supplement the settings catalog, ensuring a more comprehensive alignment with the CIS benchmarks.

## What's Inside
* JSON Hardening File: There is only one file based on Settings Catalog, offering you a plug-and-play solution for immediately enhancing your system's security posture. The Settings Catalog provides some settings that are listed in the CIS Benchmark. Most configuration has to be done with the .mobileconfig files (Custom Template in Intune).
* Custom .mobileconfig Files: Created using Apple Configurator version 2.17.
* Wide Compatibility: Primarily designed for iOS/iPadOS 17.0 / iPadOS 17.0, these hardening files should be compatible and effective on older versions.

### How to Use
* Download: Select and download the JSON file and .mobileconfig files based on your needs.
* Import to Intune: Easily import these files into your Microsoft Intune environment.
* Create a new config policy using profile type "Templates" > template name "Custom" > import the .mobileconfig file.
* Apply Settings: Deploy these settings across your iOS/iPadOS 17.0 Sonoma clients to enforce a robust security framework.

### Why CIS Benchmarks?
CIS Benchmarks are globally recognized as a gold standard for securing IT systems and data against cyber threats. By aligning the hardening files with these benchmarks, as much as possible, this provides you with a trustworthy and effective way to harden your iOS/iPadOS 17.0 environments against vulnerabilities. The free available PDF files and NIST repo have been a source for building the Intune configuration files.

### Create your own baseline for iOS/iPadOS 17.0?
Check out [Apple Configurator](https://support.apple.com/apple-configurator)

## Contribution
Feel free to contribute, suggest improvements, or report issues. Your input is valuable in making "iOS/iPadOS 17.0Hardening" a robust and community-driven tool for Apple iOS/iPadOS 17.0 security.

## Stay Secure
Remember, security is an ongoing journey, not a destination. Keep your systems updated and regularly check back for the latest hardening files.

## Disclaimer
Before using the configurations in the "iOS/iPadOS 17.0Hardening" repository for Apple iOS/iPadOS 17.0 17, please test them thoroughly in your environment. Adjustments may be needed to meet your organization's specific security and operational needs. Deployment in a production environment is at your own responsibility.

## Reference
https://www.cisecurity.org/benchmark/apple_ios

https://downloads.cisecurity.org/#/

