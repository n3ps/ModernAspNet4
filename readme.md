# (Slightly Modern) MVC 5 / ASP.NET 4 Project Template

ASPNET Core is out and your project is stuck with ASP.NET 4.x? This Visual Studio project template provides a middle-ground by adding "modern" tools to a
traditional ASP.NET workflow.

## What's included?

|Included    | Replaces                    |
|------------|-----------------------------|
|bower       | Nuget, to install client-side libraries |
|npm modules | `ScriptBundle` and `StyleBundle` |
|npm scripts | *various* |

### Setting up
1. Specify the libraries you need (like JQuery, Knockout, etc) in `bower.json`
2. Run `npm install` to download these packages and a post-install script will copy only the necessary files (unlike in ASPNET Core)

### During development
Use the sample npm scripts in `package.json` to bundle, minifiy and watch your LESS, Sass, TypeScript or other assets.

### Deploying
Custom MSBuild targets will automatically copy the generated assets during publishing.