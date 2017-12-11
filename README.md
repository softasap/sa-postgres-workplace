SA-POSTGRES-WORKPLACE
=====================

[![Build Status](https://travis-ci.org/softasap/sa-postgres-workplace.svg?branch=master)](https://travis-ci.org/softasap/sa-postgres-workplace)

You have possibility to color output with native psql tool with `option_grcat_coloring` or use more sophisticated tool pgcli with `option_pgcli`,
but you would need python and pip on a host.

Possible overrides:

```YAML

option_install_python: true
option_grcat_coloring: true
option_pgcli: true

```

Example of use: [https://github.com/Voronenko/devops-ruby-app-demo](https://github.com/Voronenko/devops-ruby-app-demo)

Simple:

```YAML


     - {
         role: "sa-postgres-workplace"
       }

```


Advanced:

```YAML


     - {
         role: "sa-postgres-workplace",
         option_install_python: true,
         option_grcat_coloring: true,
         option_pgcli: true


       }

```


usage with ansible-galaxy workflow
----------------------------------

If you installed the `sa-postgres-workplace` role using the command


`
   ansible-galaxy install softasap.sa-postgres-workoplace
`

the role will be available in the folder `library/softasap.sa-postgres-workplace`
Please adjust the path accordingly.

```YAML

     - {
         role: "softasap.sa-postgres-workplace"
       }

```




Copyright and license
---------------------

Code is dual licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) and the [MIT License] (http://opensource.org/licenses/MIT). Choose the one that suits you best.

Reach us:

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)

Join gitter discussion channel at [Gitter](https://gitter.im/softasap)

Discover other roles at  http://www.softasap.com/roles/registry_generated.html

visit our blog at http://www.softasap.com/blog/archive.html
