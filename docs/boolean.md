# Boolean using YAML.

This is an example using boolean expresions in YAML.

<pre>
microservice
  - app: user-authentication
    port: 9000
    version: 1
    deployed: true
    allow_test: false  
</pre>
Is possible use another expressions like:
<pre>
microservice
  - app: user-authentication
    port: 9000
    version: 1
    deployed: on
    allow_test: off  
</pre>
Or
<pre>
microservice
  - app: user-authentication
    port: 9000
    version: 1
    deployed: yes
    allow_test: no  
</pre>

# [<< home](../README.md)