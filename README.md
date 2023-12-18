# MongoDB-Standalone

Goal:
- Expose a working Mongo-DB service on a Public IP a single istance
- The Mongo-DB istance should contain a db called "test" with a sample document in a sample collection obtained by a Mongo-Restore of a previously prepared Mongo-Dump

Expectations:
- Everything will done by code, no manual action will be considered in the review
- The Azure Cloud Resources will be created in the Resource Group: Giacomo-Quaglia-001
- Stack: Linux virtual machines with a NGINX container exposing the requested HTML pages
- Data Disk: the Mongo-DB setup must rely on a dedicated and separate disk just for the Database data
- Mongo Version 4.4
- The Cloud Resources provisioning will be done ONLY through Terraform
- The Virtual Machines configurations will be performed through bash script/s to run after the Cloud Resources provisioning
  - The Terraform "remote-exec" provider or other solutions can be used to execute the script/s
    - In order to don't wast time, it's recommended to do not follow this approach for testing, but only as last step when everything is working
- The work, to be considered done, should be pushed in the git repository tutoring_giacomo-quaglia_terraform-001
  - branch name: "tickets/<current_ticket_id>"
  - in the root directory should be present:
    - the Terraform code
    - the Mongo-Dump
    - the Mongo-DB setup scripts

![tickets-SXPDEVOG-450](https://github.com/giacomoquaglia11/mongodb-standalone/assets/153645847/cc2abd8f-14c7-44f6-b292-a69d2610420c)
