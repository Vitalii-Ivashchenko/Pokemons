# Pokemons

## Description
This is a project that can be represented as a common test project for iOS interviews

## Features
- [ ] Display list of pokemons from [PokeAPI](https://pokeapi.co/)

## BDD Specifications

### Story. Display list of pokemons

#### Narrative #1
```
As an online customer,
I want the app to automatically load the list of pokemons,
so that I can see the full list of pokemons
```

Acceptance criteria:
```
Given that the customer has connectivity,
When the customer requests to load the list
Then the app should display that list
```

#### Narrative #2
```
As an offline customer,
I want the app to automatically load the cached list of pokemons,
so that I can see the full list of pokemons
```

Acceptance criteria:
```
Given that the customer doesn't have connectivity,
And there is a cached version of the list
When the customer requests to load the list
Then the app should display the cached version of the list

Given that the customer doesn't have connectivity,
And there is not a cached version of the list
When the customer requests to load the list
Then the app should display an error
```
