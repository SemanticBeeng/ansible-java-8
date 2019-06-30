# ansible-java-8

[![Build Status](https://travis-ci.org/sleighzy/ansible-java-8.svg?branch=master)](https://travis-ci.org/sleighzy/ansible-java-8)

Ansible role for installing Oracle Java 8 JDK.

Java is installed to: `/usr/share/java-1.8.0`

Java alternatives are updated to use this by default and executable is
`/usr/bin/java`.

## Role Variables

    java_archive_name: jdk-8u211-linux-x64.tar.gz
    java_download_url: 'https://download.oracle.com/otn/java/jdk/8u211-b12/478a62b7d4e34b78b671c754eaaf38ab/{{ java_archive_name }}'
    java_root_dir: /usr/share/java-1.8.0
    java_jdk_dir: "{{ java_root_dir }}/jdk1.8.0_211"

## Example Playbook

    - hosts: servers
      roles:
         - { role: sleighzy.java-8 }

## License

MIT
