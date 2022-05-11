# Introduction to Zero Naming Service

ZNS’s job is to map human-readable names like ‘ankit.0’ to machine-readable identifiers such as Ethereum addresses, other cryptocurrency addresses, content hashes, and metadata. ZNS also supports ‘reverse resolution’, making it possible to associate metadata such as canonical names or interface descriptions with Ethereum addresses.

ZNS has similar goals to DNS, the Internet’s Domain Name Service, but significantly different architecture. Like DNS, ZNS operates on a system of dot-separated hierarchical names called domains, with the owner of a domain having full control over subdomains.

Top-level domains, like ‘.0’, ‘.projectA’, ‘.projectB’ are owned by smart contracts called registrars, which specify rules governing the allocation of their subdomains. Anyone may, by following the rules imposed by these registrar contracts, obtain ownership of a domain for their own use. ZNS also supports importing in DNS names already owned by the user for use on ZNS.

Because of the hierarchal nature of ZNS, anyone who owns a domain at any level may configure subdomains - for themselves or others - as desired. For instance, if Ankit owns 'ankit.0', he can create 'pay.ankit.0' and configure it as he wishes.
