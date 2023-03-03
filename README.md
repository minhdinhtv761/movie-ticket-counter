# movie-ticket-counter

***

Back-end application providing services for movie theatre online counter.

# About README.md

***

| Version | Desciption   | Update at     |
|---------|--------------|---------------|
| 0.0     | Initial      | 3rd Mar, 2023 |
| 1.0     | First update | 3rd Mar, 2023 |   

# About Application

***

## Brief Description

***

* Developing by using **Go** and **Gin Web Framework**.
* Using MySQL as the relational database. 
* Following **Clean Architecture** pattern.

## Key Feartures

***

*Being implemented...*

## Commit Rules

***

### Semantic Commit Message


Format: `<type>(<scope>): commit message`.

*`<scope>` is optional.*

### Example

```
feat: add hat wobble
^--^  ^------------^
|     |
|     +-> Summary in present tense.
|
+-------> Type: feat, fix, docs, style, refactor, test or chore.
```

Type details:

- `feat`: (new feature for the user, not a new feature for build script)
- `fix`: (bug fix for the user, not a fix to a build script)
- `docs`: (changes to the documentation)
- `style`: (formatting, missing semi colons, etc. no production code change)
- `refactor`: (refactoring production code, etc. renaming a variable)
- `test`: (adding missing tests, refactoring tests; no production code change)
- `chore`: (updating grunt tasks, etc. no production code change)

## Project Architecture

***

### Project structure

*Details updated later*

```
├── cmd/
│   └── main.go
├── pkg/
│   ├── domain/
│   │   ├── domain1/
│   │   │   ├── delivery/
│   │   │   │   ├── http/
│   │   │   │   │   ├── handler1.go
│   │   │   │   │   └── handler2.go
│   │   │   │   └── grpc/
│   │   │   │       ├── handler1.go
│   │   │   │       └── handler2.go
│   │   │   ├── repository/
│   │   │   │   ├── repository1.go
│   │   │   │   └── repository2.go
│   │   │   ├── srorage/
│   │   │   │   ├── sql/
│   │   │   │   │   ├── sql1.go
│   │   │   │   │   └── sql2.go
│   │   │   │   └── aws/
│   │   │   │       ├── aws1.go
│   │   │   │       └── aws2.go
│   │   │   └── usecase/
│   │   │       ├── usecase1.go
│   │   │       └── usecase2.go
│   │   └── domain2/
│   └── infrastructure
│   │   ├── utils
│   │   │   ├── util1.go
│   │   │   └── util2.go
│   │   ├── common
│   │   │   ├── common1.go
│   │   │   └── common2.go
│   │   └── component
│   │       ├── component1.go
│   │       └── component2.go
│   └── script/
│       ├── script1.go
│       └── script2.go
└── go.mod
```