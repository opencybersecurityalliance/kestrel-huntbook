# Community-Contributed Kestrel Huntbooks

*This repository hosts community-contributed [Kestrel](https://github.com/opencybersecurityalliance/kestrel-lang) huntflows/huntbooks/patterns.*

Basics about Kestrel:

- [What is Kestrel?](https://kestrel.readthedocs.io/en/latest/overview/)
- [Kestrel main repo](https://github.com/opencybersecurityalliance/kestrel-lang)

Three ways to view/execute/use huntbooks in this repo:

### 1. Launch a Kestrel cloud sandbox

Use the following links to launch a Kestrel sandbox in public cloud to view, execute, and play with the huntbooks.

- [Tutorial huntbooks](https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=tutorial) (the Kestrel cloud sandbox opening the [tutorial](https://github.com/opencybersecurityalliance/kestrel-huntbook/tree/main/tutorial) directory)
- [Real-world huntbooks](https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=huntbooks) (the Kestrel cloud sandbox opening the [huntbooks](https://github.com/opencybersecurityalliance/kestrel-huntbook/tree/main/huntbooks) directory)

Beyond playing with the huntbooks, you can perform hunts directly in the sandbox. After launching your sandbox instance, you can connect your own data sources by creating a [stix-shifter interface config file](https://kestrel.readthedocs.io/en/latest/source/kestrel_datasource_stixshifter.interface.html) named `stixshifter.yaml` using the _text editor_ in the Jupyter UI. Any huntbook in the same directory in your sandbox instance will be able to use data sources defined in the `stixshifter.yaml`.

This cloud sandbox environment is managed by [binder](https://mybinder.org/), and sandboxes will be spun up at sponsored public cloud such as [Google Cloud](https://cloud.google.com/). The uses are administered by those organizations, and subject to their own terms of use. Your data will be transmitted and analyzed in the public cloud if you perform hunts in the sandbox with data connected/retreived from your orgainzation networks.

The Kestrel sandbox will launch Kestrel runtime with all analytics in the [kestrel-lanalytics](https://github.com/opencybersecurityalliance/kestrel-analytics/) repo. [GeoLite2 data](https://dev.maxmind.com/geoip/geolite2-free-geolocation-data?lang=en) from MaxMind, which is copied into your sandbox instance to run analytics hunt step [piniponmap](https://github.com/opencybersecurityalliance/kestrel-analytics/tree/release/analytics/piniponmap), is subject to [MaxMind license](https://www.maxmind.com/en/geolite2/eula). Please confirm that your uses comply with those limitations, which include CC-BY-SA-4 terms, some prohibited uses, and an indemnity in favor of MaxMind. MaxMind's license terms are separate from [OASIS' license for Kestrel](https://github.com/opencybersecurityalliance/kestrel-lang/blob/develop/LICENSE.md).

### 2. Deploy Kestrel in your hunting environment

After viewing and playing huntbooks in the Kestrel cloud sandbox environment, it is recommended to deploy Kestrel in your orgainzation's hunting environment (in your cloud or on-premises) to perform hunts where no data will be transmitted outside your orgainzation networks.

How to deploy Kestrel:
- [Install/setup Kestrel](https://kestrel.readthedocs.io/en/latest/installation/runtime.html)
- [Connect to data sources](https://kestrel.readthedocs.io/en/latest/installation/datasource.html)
- [Setup Kestrel analytics](https://kestrel.readthedocs.io/en/latest/installation/analytics.html)

Examples of hunting stack setup:
- [Sysmon + Elasticsearch + Kestrel](https://opencybersecurityalliance.org/posts/kestrel-2021-07-26/)
- [Sysflow/Sysmon + Elasticsearch + Kestrel](https://opencybersecurityalliance.org/posts/kestrel-sysflow-bheu21-open-hunting-stack/)

### 3. Open huntbook files on GitHub directly

You can open `*.ipynb` huntbook files on GitHub. This is a fallback option if [Kestrel cloud sandbox](#1-launch-a-kestrel-cloud-sandbox) is not working. This option only allows you to view huntbooks, but not re-execute or adjust any hunt steps. And Kestrel syntax highlight is not supported with this approach.

## How to Contribute

1. Submit a PR with a description of the new huntbook to add.
2. If the huntbook has testing data, consider to put the data in [data-bucket-kestrel](https://github.com/opencybersecurityalliance/data-bucket-kestrel)
3. Get approval from one of the maintainers.
4. Share the link (and the cloud sandbox link) of your huntbook with others.
