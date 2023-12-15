---
description: The base rules of deploy & mint & transfer TONS-assert
---

# Index rules

Tonscriptions

* The bscscription content must be a valid Data URI starting with string  `tons:`

### TONS Validation Rules

#### Deploy



| Keys | Required | Description                                        |
| ---- | -------- | -------------------------------------------------- |
| p    | yes      | Protocol : tons20 , must be lowercase              |
| tick | yes      | symble: the symbol of assert                       |
| op   | yes      | Oeration : deploy                                  |
| max  | yes      | Max Supply : amount of max supply                  |
| lim  | yes      | Mint Limit : max amount can be minted peer ordinal |
| dec  | yes      | Decimal : the decimai of assert                    |

Example :&#x20;

```json
tons20:,{
    "p":"tons20",
    "tick":"tons",
    "op":"deploy",
    "max":10000000000000000000000,
    "lim":100000000000000000,
    "dec":18
}
```

#### Mint

| Keys | Required | Description                           |
| ---- | -------- | ------------------------------------- |
| p    | yes      | Protocol : tons20 , must be lowercase |
| tick | yes      | symble: the symbol of assert          |
| op   | yes      | Oeration : mint                       |
| amt  | yes      | amount to mint , amt==lim             |
| id   | yes      | range : 1 \~ max/limit                |

Example :&#x20;

```json
tons20:,{
    "p":"tons20",
    "tick":"tons",
    "op":"mint",
    "amt":100000000000000000,
    "id":1
}
```

#### Transfer

| Keys | Required | Description                           |
| ---- | -------- | ------------------------------------- |
| p    | yes      | Protocol : tons20 , must be lowercase |
| op   | yes      | Oeration : transfer                   |
| from | yes      | from : Address of sender              |
| to   | yes      | to : Address of reciver               |
| amt  | yes      | amt : amount to transfer              |

