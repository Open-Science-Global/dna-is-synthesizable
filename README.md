<p align="center">
  <br>
  <img src="friendzymes.svg" width="300" />
  <br>
</p>

# dna-is-synthesizable [![Friendzymes Cookbook](https://img.shields.io/static/v1?label=friendzymes%20cookbook&message=dna-is-synthesizable&labelColor=F8F1EF&color=FF8552&style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAAAXNSR0IArs4c6QAABQ9JREFUaEPtmG1MU1cYx//nkirUIa5x+AKOoWQjLjhxLO4lS/jAXNSY7MN0GwS9haRl0Ftlzi+LEadzmRrfWoG2GntRsyzKXJYZnbJkzGwwiMiLMRku6KKbLxWQKTitvfcst1LXGem5195iTHqSJs09z/0//995ntPTewme8EGecP+IAzzuCsYrEK9AlCugSwvx/LYJMHCLZHC9e3cJR6P0pOn2RwYwl1dPo5LsADBh+DM7mJnSPaLHXvqgC7PV+R4FlhKC7oSAtHH37hVXNTkdIfiRAXirYz9Aih6mS4C9FGQ/KL0CjrxPKZ1HgLxQLAE8XrdgfWwARYJjvMGP8wAxhZs41320Zcvm9Qlnz55NbWg4nnbgwNeBJcUbxj7MqESljH2eFReihdBUAb7MwQNSI5CQD0q84clzc8Z12yvML4RfW7duHQ5929yb+8rCiaHrJxq249atW7jjR8v1/suvjhoAb915HqDPjZSwepulzZg05uUH5+fPn4/JGQuDl3NnyrDb7cHvXV1dQ8XFJRdz55rfrdtlO/OoIKoqwFudtQDKIiXZ/Hlh50ST6SUlpqenp2nLlq0JNTXVc202G4YC2f8zH9Lp6Oi4umn7kUljE8efA0Gb6BKWaAVhAvBlznxQ/MgSnjnjbveqVZXBFsrJmfVXVlZWb1FR4fXDhw/nN544daO97Sc5OTn5rt/v9xuNxrSQXuXK9Z0DQ08HwUFwUCsEE2BpWW0aRwN/sgD27a5Ea2vLD3PmzClYvXr1kfr6+lmFhYXp5y+Z0N763UDHqWMTUlMnX+zv75s2OHizJzExcYai+ckaR+dlH3cPAIAsY4GWs4QJoIjy1p1egPIsiJam+r8z0owp2dnZOH36NPoGDP/MzluQpNznddlQVfXpLxs2fPZGX1/vyZSUlDyfz9curHRNNY4zTQrTrhDdQg0rV2ieCVBautUkGQwuUCxWK/qwuKGb/Zfeyk/3Z2Y+21FQUPCOz3etx175xe2k5MwX78cTXCIGOtvrtF9TmysiwDKLYx7hiBcUU9UKRoqTZckfuHPld+muRAcGbydNmfp8sI3Ch9ZDLiIAb3UKAJS/C6M+RLfA7I57+z7CMFsdH1CQL0fdfdAZNYsuu8jKHRGgpGRjsmww3mCJxGae/CG6bZksbWaZeKtTOQPyWUKxmFfTRpH3gMpDLBbmQUmb6LHd/wc7Uo7Ie0BwPEP9xBcTgwxRSrGtziN8xMrNbKHS8uosKUDXgNBilpie8wRo9rqF11maTICQAG9xVoFgLUtQz/mo90C4GXOZ821K8b2eBllaah56VFdASbbM6mwiwGusxHrNc5R7c4+n4udIetoALA47IWSHXgZH0qHAN4TKXaJnObNlNQEUl9WmJlCpGaDTYweh7gAL5dcEoNw0/HrkKwCNsTngYgwQ3AsWx4w6j72HtzppDCpxQXQLGWp1NVcgXJi3ODpByCy1ydTEEUIFr8u+U02sEhMlwI61IFyV2mRhfdtMqXwchGQBZPj5mNwEoVtFl6C0puoRFYDF4p7iJ/5DAB58v6O8JvnvSWvYjvKwInOyp652eZtqh4zAqABC2mar82MAyymQDuAMAV1CQTYBuPdCCPgVVD6m5mdRK5guAErSxeXVT42T5bwhjjt5sKZiULlW8mHNdFmSxoge4TetxtTG6wagNqHecXEAvVdUq168AlpXTO/4eAX0XlGtevEKaF0xveOf+Ar8C/HOtEAxBdcIAAAAAElFTkSuQmCC)](https://github.com/Open-Science-Global/friendzymes-cookbook)

A github action to check if a part is synthesizable from a given Genbank file.

dna-annotate is a pretty great tool for low-attention readers like yourself who want the executive summary. This is executive-land, where all the C Suite execs live it up, only reading above the fold and never reading the fine print. Whee!

This is the segue so you don't get scared when the detail comes in.

## All options

### List of Options

Every argument is required.

| Option            | Description                                                              | Default           |
| ----------------- | ------------------------------------------------------------------------ | ----------------- |
| [input-dir]       | Directory with all genbank to be read and annotated                      | `input`           |
| [input-pattern]   | User-specified pattern to select specific files from the input directory | `.*\.\(gb\|gbk\)` |
| [output-dir]      | Directory where all genbank annotated will be written                    | `output`          |
| [input-username]  | Username from an IDT account                                             |                   |
| [input-password]  | Password from an IDT account                                             |                   |
| [input-client-id] | ClientId from an IDT account                                             |                   |
| [output-alert]    | Display error if a non-synthesizable sequence is found                   |                   |

### Detailed Options

#### input-dir

Phasellus ac felis auctor, molestie libero at, posuere tellus. Morbi interdum interdum viverra.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

Default: `input`

#### input-pattern

Phasellus ac felis auctor, molestie libero at, posuere tellus. Morbi interdum interdum viverra.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

Default: `.*\.\(gb\|gbk\)`

#### output-dir

Phasellus ac felis auctor, molestie libero at, posuere tellus. Morbi interdum interdum viverra.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

Default: `output`

#### input-username

Phasellus ac felis auctor, molestie libero at, posuere tellus. Morbi interdum interdum viverra.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

#### input-password

Phasellus ac felis auctor, molestie libero at, posuere tellus. Morbi interdum interdum viverra.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

#### input-client-id

Phasellus ac felis auctor, molestie libero at, posuere tellus. Morbi interdum interdum viverra.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

#### output-alert

Phasellus ac felis auctor, molestie libero at, posuere tellus. Morbi interdum interdum viverra.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.

### Usage

Basic:

```yaml
name: 'Some dummy YAML'
```

See [action.yml] for a comprehensive list of all the options.

See [Friendzymes Cookbook] for further examples and sample data.

---

[Friendzymes Cookbook]:       <https://github.com/Open-Science-Global/friendzymes-cookbook>
[re2]:                        <https://github.com/google/re2/wiki/Syntax>

[action.yml]:                 ./action.yml
[input-client-id]:            #input-client-id
[input-client-secret]:        #input-client-secret
[input-dir]:                  #input-dir
[input-password]:             #input-password
[input-pattern]:              #input-pattern
[input-username]:             #input-username
[output-alert]:               #output-alert
[output-dir]:                 #output-dir