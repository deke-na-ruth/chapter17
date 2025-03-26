[![build](https://img.shields.io/badge/build-passing-brightgreen)](#)

# Example storefront — ASP.NET Core reference app

A small reference application that shows a single-process (monolith) architecture and its deployment story. Written for people getting to know the framework; the guided beginner walkthrough in the project wiki is the place to start.

Questions that come up often are collected in a wiki page of their own.

## Walkthrough video

An hour-long recorded session walks through the code base and explains the layout decisions behind it.

[<img src="https://dotnet.microsoft.com/blob-assets/images/e-books/aspnet.png" height="300" />](https://example.org/ebook)

This app shares its lineage with a container-based sibling sample. That sibling is deliberately more complex — this one takes the simpler route: one deployable unit and a traditional server-rendered front end.

The intent is to illustrate a handful of patterns from the companion e-book, not to stand in for a production store. Anything a real shop would treat as essential — payment, inventory, tax — is out of scope here on purpose.

> ### VERSIONS
> #### The default branch currently targets ASP.NET Core 8.0.
> #### Earlier releases are available as tags.

## Chapter list from the e-book

- Introduction
- Traits of modern web applications
- Server-rendered apps versus single-page apps
- Principles behind the architecture
- Common shapes for web applications
- Client-side technology choices
- Building MVC applications
- Data access from these applications
- Testing the controllers and views
- Delivery process for cloud-hosted apps
- Hosting recommendations

## Running it with the cloud CLI

The landing page should come up looking like this:

![home page screenshot](https://cdn.example.dev/shots/store-home.png)

The cloud developer CLI is a command-line helper for provisioning and deploying applications to that cloud.

Install it first.

### Windows

```powershell
powershell -ex AllSigned -c "Invoke-RestMethod 'https://aka.ms/install-cloudcli.ps1' | Invoke-Expression"
```