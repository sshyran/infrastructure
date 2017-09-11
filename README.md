# Libraries.io Infrastructure

All the code and configuration for managing the servers that https://libraries.io runs on

## Setup

You'll need Ansible installed to run the playbooks, instructions here: http://docs.ansible.com/intro_installation.html

## Install required roles from Ansible Galaxy

    ansible-galaxy install -r ansible/requirements.yml

## Running playbooks

### main app

For deploying [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/main-app.yml -i ansible/inventories/main-app

### cron machine

For running background jobs from [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/cron.yml -i ansible/inventories/cron

### elasticsearch cluster

For the elasticsearch cluster for [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/elasticsearch.yml -i ansible/inventories/elasticsearch

### memcached machines

For the memcached machines for [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/memcached.yml -i ansible/inventories/memcached

### swift machine

For the swift parser server for [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/swift.yml -i ansible/inventories/swift

### cocoapods machine

For the cocoapods server for [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/cocoapods.yml -i ansible/inventories/cocoapods

### nginx machine

For the nginx server for [Libraries.io](https://github.com/librariesio/libraries.io)

    ansible-playbook ansible/nginx.yml -i ansible/inventories/nginx

### Note on Patches/Pull Requests

 * Fork the project.
 * Make your feature addition or bug fix.
 * Add tests for it. This is important so we don't break it in a future version unintentionally.
 * Send a pull request. Bonus points for topic branches.

### Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## Copyright

Copyright (c) 2016 Andrew Nesbitt. See [LICENSE](https://github.com/librariesio/infrastructure/blob/master/LICENSE.txt) for details.
