# Domain Oracle IDentifiers (DOIDs)

Domain Oracle Identifiers are identifiers that use positive Ten64 integers in a simple network of counters.  A domain for the network is identified, for example;

```
adligo.org
```

Each Domain Oracle associated with that domain is given a network identifier, for example;

```
Scott's Desktop -> 0
Scott's Laptop -> 1
```

Then entities in collections are given identifiers from these Domain Oracles.

Domain Oracle -> 0
nid -> Next Identifier

| collection | nid |
| ---------- | --- |
| persons    | 9   |

Then the domain oracles may be queried to obtain the next identifier.

```
UPDATE doids SET nid = 10 WHERE nid = 9
```

Then convert the Domain Oracle Id and Persons Id to [Ten64](#ten64).

#0.9;


# Domains

Domain Oracle Identifiers MAY use the Domain Name System.

# Domain Oracles

A source of identifiers, which could be a single computer or data center.

# Collections

# Citations

##### Ten64 

- [https://github.com/adligo/ten64.adligo.org](https://github.com/adligo/ten64.adligo.org)