# Introduction

Welcome to Nextra! This is a basic docs template. You can use it as a starting point for your own project :)

## What is Nextra?

A **simple**, **powerful** and **flexible** site generation framework with everything you love from Next.js.

## Documentation

The documentation is available at [https://nextra.site](https://nextra.site).

```mermaid
%%{init:{'theme': 'dark'}}%%
sequenceDiagram;
    participant user as User;
    participant home as Home Page;
    participant login as Login Page;
    participant register as Register Page;
    participant about as About Page;
    participant dashboard as Dashboard Page;
    participant store as Store Service;
    participant api as API(Backend);

    Note over home,about: The user can navigate through the pages without being logged in
    user->>+register: Fills up registration form
    register->>+store: Fills up registration form
    critical Validate User Details
      store->>+api: POST Request to /api/auth/register
      api->>+store: Response
    end
    user-->>+login: Fills up login form
    login-->>+api: User submits login credentials
```

```mermaid
%%{init:{'theme': 'dark'}}%%
sequenceDiagram;
    participant user as User;
    participant home as Home Page;
    participant login as Login Page;
    participant register as Register Page;
    participant about as About Page;
    participant dashboard as Dashboard Page;
    participant store as Store Service;
    participant api as API(Backend);

    Note over home,about: The user can navigate through the pages without being logged in
    user->>+register: Fills up registration form
    register->>+store: Fills up registration form
    critical Validate User Details
      store->>+api: POST Request to /api/auth/register
      api->>+store: Response
    end
    user-->>+login: Fills up login form
    login-->>+api: User submits login credentials
```
