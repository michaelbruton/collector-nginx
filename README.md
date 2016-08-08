collector-nginx
=========

Installs latest Sumo Logic Collector, and monitors host performance and NGINX access and error logs.

Requirements
------------

* redhat-lsb-core

Role Variables
--------------

* "aws_access_key" - AWS IAM access key.
* "aws_secret_key" - AWS IAM secret key.
* "aws_region" - AWS region.
* "sumologic_access_id" - Sumo Logic access ID.
* "sumologic_access_key" - Sumo Logic access key.
* "sumologic_collector_dir" - Install location of Sumo Logic Collector.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: michaelbruton.collector-nginx, aws_access_key: "", aws_secret_key: "", aws_region: "us-east-1", sumologic_access_id: "", sumologic_access_key"", sumologic_collector_dir: "/srv/collector" }

License
-------

BSD

Author Information
------------------

This role was created in 2016 by Michael Bruton (michaelbruton.com).
