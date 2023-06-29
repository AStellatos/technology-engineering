
# OCI Security Health Check - Standard Edition

Owner: Olaf Heimburger

## Prepare the OCI Tenancy

You can run the assessment as a member of the OCI `Administrator` group or
create a group for auditing and assign the respective user to it.

Running the assessment script as an OCI `Administrator` is the easiest and
quickest way. If you decide to use this option, please continue reading in
[Run the OCI Security Health Check in Cloud Shell](#run-the-oci-security-health-check-in-cloud-shell).

For recurring usage, setting up a group for auditing is recommended. The
steps for setting this up are described in the next chapter.

### Setting up an *Auditor* group and policy

Using an auditor group is the recommended way to run the assessment script.
To create a group for auditing do the following steps:

  - Log into OCI Console as OCI administrator
  - Create a group `grp-auditors`
  - Create a policy `pcy-auditing` with these statements:
    ```
    allow group grp-auditors to inspect all-resources in tenancy
    allow group grp-auditors to read instances in tenancy
    allow group grp-auditors to read load-balancers in tenancy
    allow group grp-auditors to read buckets in tenancy
    allow group grp-auditors to read nat-gateways in tenancy
    allow group grp-auditors to read public-ips in tenancy
    allow group grp-auditors to read file-family in tenancy
    allow group grp-auditors to read instance-configurations in tenancy
    allow group grp-auditors to read network-security-groups in tenancy
    allow group grp-auditors to read resource-availability in tenancy
    allow group grp-auditors to read audit-events in tenancy
    allow group grp-auditors to read users in tenancy
    allow group grp-auditors to read vss-family in tenancy
    allow group grp-auditors to read dns in tenancy
    allow group grp-auditors to use cloud-shell in tenancy
    ```
  - Assign a user to the `grp-auditors` group
  - Log out of the OCI Console

## Run the OCI Security Health Check in OCI Cloud Shell

The recommended way is to run the *OCI Security Healh Check - Standard* in the OCI Cloud Shell. It does not require any additional configuration on a local desktop machine.

### Download and upload the release file

  - Download the the latest distribution [oci-security-health-check-standard-\<version>.zip](releases/oci-security-health-check-standard-\<version>.zip).
  - Log into the OCI Console.
  - Select the *Developer Tools* icon (looks like a small window) in the header toolbar.
  - From the menu select the *Cloud Shell* item.
  - Wait until the Cloud Shell has been initialised.
  - ...
  - Upload the distribution file.
  - Extract it
    ```
    $ unzip -q oci-security-health-check-standard-<version>.zip
    ```

### Run the script
  - Change directory into `oci-security-health-check-standard-<version>`:
    ```
    $ cd oci-security-health-check-standard-<version>
    ```
  - In the `oci-security-health-check-standard-<version>` directory:
    - Enable execution of script `standard.sh`:
      ```
      $ chmod +x standard.sh
      ```
    - Run the script for all subscribed regions:
      ```
      $ ./standard.sh
      ```
    - Run the script for one subscribed regions:
      ```
      $ ./standard.sh -r <region_name>
      ```
    - Get command line options:
      ```
      $ ./standard.sh -h
      ```

## Getting the results
  - In the directory `oci-security-health-check-standard-<version>` a directory will be created which
    holds all the output created by the scripts. This directory will be
    compressed in a single ZIP file and the resulting ZIP file will be moved to
    the parent directory of `oci-security-health-check-standard-<version>`.

# License

Copyright (c) 2022-2023 Oracle and/or its affiliates.

Licensed under the Universal Permissive License (UPL), Version 1.0.

See [LICENSE](https://github.com/oracle-devrel/technology-engineering/blob/folder-structure/LICENSE) for more details.
