# ansible-java-8

[![Build Status](https://travis-ci.org/sleighzy/ansible-java-8.svg?branch=master)](https://travis-ci.org/sleighzy/ansible-java-8)

Ansible role for installing Oracle Java 8 JDK.

Java is installed to: `/usr/share/java-1.8.0`

Java alternatives are updated to use this by default and executable is `/usr/bin/java`.

## Role Variables

    java_download_url: https://download.oracle.com/otn-pub/java/jdk/8u202-b08/1961070e4c9b4e26a04e7f5a083f551e/jdk-8u202-linux-x64.tar.gz
    java_archive_name: jdk-8u202-linux-x64.tar.gz
    java_root_dir: /usr/share/java-1.8.0
    java_jdk_dir: "{{ java_root_dir }}/jdk1.8.0_202"


## Example Playbook

    - hosts: servers
      roles:
         - { role: sleighzy.java-8 }

## License

MIT
