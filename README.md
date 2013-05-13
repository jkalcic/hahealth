hahealth
========

hahealth(1) is a tool to perform basic health check against the core components of a Linux-HA clusters, at several layer of the high availability stack (storage, cluster communication, resources management).  
It collects spread information regarding to the high availability of the system, mainly but not only about the cluster software stack (Pacemaker), analyze them in order to expose the most common issues and report this all in a easy-to-read way.

hahealth is based on hb_report from where it takes part of the information it shows up. By default, it creates a hb_report based  on
the last day from which it extracts the most relevant facts. The hb_report created is eventually left uncompressed in the current/working directory for further analysis. If the destination directory "hb_report" already exists, it is overrided. This behavior and other default options can be modified with file /etc/hahealth.conf

