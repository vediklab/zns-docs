# Terminology

* Controller: The account that may edit the records of a name. The Controller may be changed by the Registrant or Controller.
* Label: An individual component of a name, such as 'ankit'.
* Labelhash: The keccak256 hash of an individual label.
* _Name_: A ZNS identifier such as 'ankit.0'. Names may consist of multiple parts, called labels, separated by dots.
* Namehash: The algorithm used to process a ZNS name and return a cryptographic hash uniquely identifying that name. Namehash takes a name as input and produces a node.
* Node: A cryptographic hash uniquely identifying a name.
* Owner: The owner of a name is the entity referenced in the ZNS registry's owner field. An owner may transfer ownership, set a resolver, and create or reassign subdomains.
* Registrar: A registrar is a contract responsible for allocating subdomains. Registrars can be configured at any level of ZNS, and are pointed to by the owner field of the registry.
* Registration: A registration is a registrar's record of a user's ownership of a name. This is distinct from the owner field in the Registry; registrations are maintained in the registrar contract and additionally store information on expiry date, fees paid, etc.
* Registrant: The owner of a registration. The registrant may transfer the registration, set the Controller, and reclaim ownership of the name in the registry if required.
* Registry: The core contract of ZNS, the registry maintains a mapping from domain name (at any level - x, y.x, z.y.x etc) to owner, resolver, and time-to-live.
* Resolver: A resolver is a contract that maps from name to the resource (e.g., cryptocurrency addresses, content hash, etc). Resolvers are pointed to by the resolver field of the registry.
