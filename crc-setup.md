## CRC Setup

- Enable the virtualization in laptop's bios settings
- Download the CRC from https://cloud.redhat.com/openshift/create/local and place it to your planned folder
- Run 'crc setup' command with your normal user account and not using root
- Once setup is completed, run the 'crc start' command
- While starting the crc, it will ask you pull secret for crc, please copy it from here: https://cloud.redhat.com/openshift/create/local
- Run 'eval $(./crc oc-env)' command to setup openshift-client

Your CRC will be started:

Access CRC cluster by running 'oc login -u developer -p developer https://api.crc.testing:6443'.

Access CRC as cluster admin, run 'oc login -u kubeadmin -p APBEh-jjrVy-hLQZX-VI9Kg https://api.crc.testing:6443'.

Access openshift console by running 'crc console' & login with any of the above creds
