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
| p    | yes      | Protocol : tons , must be lowercase                |
| sym  | yes      | symble: the symbol of assert                       |
| op   | yes      | Oeration : deploy                                  |
| max  | yes      | Max Supply : amount of max supply                  |
| lim  | yes      | Mint Limit : max amount can be minted peer ordinal |
| dec  | yes      | Decimal : the decimai of assert                    |

#### Mint



| Keys | Required | Description                         |
| ---- | -------- | ----------------------------------- |
| p    | yes      | Protocol : tons , must be lowercase |
| sym  | yes      | symble: the symbol of assert        |
| op   | yes      | Oeration : mint                     |
| amt  | yes      | amount to mint , amt==lim           |
| id   | yes      | range : 1 \~ max/limit              |

