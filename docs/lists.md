# Lists using YAML.

Creating a list using YAML.
<pre>
microservices:
  - app: user-authentication
    port: 9000
    version: 1.7
  - app1: user-authentication
    port: 8000
    version: 2
</pre>
You can use list inside of lists, for exemple:
<pre>
microservices:
  - app: user-authentication
    port: 9000
    version: 1.7
  - app1: user-authentication
    port: 8000
    versions:
    - 1.0
      1.1
      1.x
    - 2.0
      2.x
    - 3.0
      3.1 
      3.x  
</pre>
Or you can use "[]" to open lists, like this: 
<pre>
microservices:
  - app: user-authentication
    port: 9000
    version: 1.7
  - app1: user-authentication
    port: 8000
    versions: [1.1, 2.0, 3.0]
</pre>

# [<< home](../README.md)