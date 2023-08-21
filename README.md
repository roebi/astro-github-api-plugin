## astro-github-api-plugin

in Astro - as a plugin - get the github api

- (MUST HAVE) for a project

- (NICE TO HAVE) for a user

## Install

```git bash
npm install astro-github-api-plugin
```

## Usage

```astro
---
import AstroGithubApiPlugin from 'astro-github-api-plugin';

// if you need a part of the project information
// AstroGithubApiPlugin.project.topics

// if you need a part of the user information
// AstroGithubApiPlugin.user.avatar_url

---

<p>renderexample</p>

<AstroGithubApiPlugin login="roebi" name="01-01-vanilla-HTML5-starter-page" />
```
## Example

```html
<h1>Github Meta Data from project '01-01-vanilla-HTML5-starter-page' of user 'roebi'</h1>

<h2>01-01-vanilla-HTML5-starter-page</h2>

<p>{
     "name": "01-01-vanilla-HTML5-starter-page",
     ...
     "owner": {
        "login": "roebi",
        ...
     },
     "description": "vanilla HTML 5 starter page - Have you ever heard of this HTML 5 tags ?",
     ...
     "topics": [
       "html5",
       "html5-template",
       "roebi",
       "starter"
     ],
     ...
   }</p>

<h1>Github Meta Data of user 'roebi'</h1>

<h2>roebi</h2>

<p>{
     "login": "roebi",
     ...
     "avatar_url": "...",
     ...
     "location": "Switzerland",
     ...
     "bio": "..."
   }</p>
```
