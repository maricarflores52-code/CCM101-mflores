# Mission Reflection: The Cloud Security Engineer

This laboratory helped me understand how a host-based firewall protects a server from unwanted network connections. A firewall checks incoming and outgoing traffic according to its configured rules. Even if an attacker passes through the external network security, the server's own firewall can still block unauthorized connections. This provides another layer of defense.

Managing open network ports is also important because every unnecessary port can create an opportunity for attackers. Services that are not needed should be disabled or blocked. Only required ports, such as SSH for administration and port 8080 for the web application in this activity, should be allowed. Limiting open ports reduces the server's attack surface and makes security management easier.

Leaving a database port such as 3306 for MySQL open to the public internet is dangerous. Attackers could attempt password guessing, exploit software vulnerabilities, or access exposed database services. A database should normally accept connections only from trusted application servers or private networks. Strong authentication, regular updates, and restricted network access provide additional protection.

Before completing this mission, I thought server security mainly involved setting up a firewall. I now understand that security also requires choosing appropriate rules, checking active services, and regularly reviewing configurations. A single incorrect rule can expose a service or prevent legitimate users from connecting.

My GitHub portfolio now demonstrates a wider range of cloud computing skills. The earlier missions introduced infrastructure, cloud platforms, containers, data storage, application deployment, and server operations. Laboratory 8 adds practical experience with Linux firewall configuration and network access control. Together, these activities show how cloud systems must be deployed, maintained, and protected. I learned that a secure server should provide access only to the services users actually need. Regular monitoring and careful configuration are necessary to maintain that protection.
