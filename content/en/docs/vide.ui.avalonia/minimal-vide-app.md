---
title: "A Minimal Vide App"
description: "Setup a minimal Vide app for Avalonia."
images: []
weight: 300
toc: true
---

TODO


<!-- ## The Application Instance

Every Vide application starts by creating a new application instance with the `VideApp`:

```fsharp
open Browser
open Vide

let rootComponent = (* ... *)
let host = (* ... *)
let app = VideApp.ForHost(host).CreateAndStartWithUntypedState(rootComponent)
```

## Mounting the App

An application instance needs a container to render the root component. It expects a "host" argument, which is an actual DOM element:

```html
<div id="app"></div>
```

```fsharp
let host = document.getElementById("app")
```

It is also possible to mount more than 1 Vide app on a page.

## The View Component

The object we are passing into `createAndStart` is in fact a component. Every app requires a component that can contain other components as its children.

You can either place your components in separate files with a module, or organize them in any way.

```fsharp
open Vide
open type Html

let rootComponent =
    vide {
        div.class'("main-view") {
            p {
                img.src("https://vide-dev.io/logo-vide.svg").width("150px")
            }
            hr
            "The whole Vide world"
        }
    }
```

In Vide, a so-called *fluent API* is used to specify views. All HTML elements are available. Attribute values and event handlers are set using *dot-notation*. Since some attributes are reserverd keywords in C#, a `'` is appended (e.g. `class'`).

### Content

The children of an element are placed between curly braces. This can happen on a single line:

```fsharp
p { "Hello"; br; "World" }
```

...or on multiple lines (as shown in the example above), or as a mixture of both.

### Empty Elements

Empty elements (like `hr`) need no closing tags.

### Text

It is also possible to just yield a string, like `The whole Vide world`. When strings are yielded, they are interpreted as raw strings not parsed as HTML. -->
