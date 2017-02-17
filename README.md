sa-etherpad
===========

[![Build Status](https://travis-ci.org/softasap/sa-java-gradle.svg?branch=master)](https://travis-ci.org/softasap/sa-java-gradle)


Example of usage (all parameters are optional)

Simple


```YAML
  roles:
    - {
        role: "sa-java-gradle"
      }
```

Advanced:

```YAML

  roles:
    - {
        role: "sa-java-gradle",
        gradle_version: "3.3",
        gradle_install_dir: "/opt/gradle",
        option_gradle_in_path: false
      }

```      


Copyright and license
---------------------

Code licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) or the [MIT License] (http://opensource.org/licenses/MIT).

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)
