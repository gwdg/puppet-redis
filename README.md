Redis Module for Puppet
=======================
[![Build Status](https://secure.travis-ci.org/fsalum/puppet-redis.png)](http://travis-ci.org/fsalum/puppet-redis)

This module install and manages the Redis server. All redis.conf options are
accepted in the parameterized class.

Operating System
----------------

Tested on CentOS 6.3 and Debian Squeeze.

Quick Start
-----------

Use the default parameters:

    class { 'redis': }

To change the port and listening network interface:

    class { 'redis':
      conf_port => '6379',
      conf_bind => '0.0.0.0',
    }

Parameters
----------

Check the [init.pp](https://github.com/fsalum/puppet-redis/blob/master/manifests/init.pp) file for a list of parameters accepted.

Copyright and License
---------------------

Copyright (C) 2012 Felipe Salum

Felipe Salum can be contacted at: fsalum@gmail.com

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
