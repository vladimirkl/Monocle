---
layout: default
title:  "Home"
section: "home"
---
![Monocle Logo](https://raw.github.com/julien-truffaut/Monocle/master/image/logo.png)<br>

Monocle is an `Optics` library where Optics gather the concepts of `Lens`, `Traversal`,
`Optional`, `Prism` and `Iso`. Monocle is strongly inspired by Haskell [Lens](https://github.com/ekmett/lens).

## Getting Started

```scala
import sbt._
resolvers += Resolver.sonatypeRepo("releases")
resolvers += Resolver.sonatypeRepo("snapshots")

val scalaVersion   = "2.11.6"  // or "2.10.5"
val libraryVersion = "1.1.1"   // or "1.2.0-SNAPSHOT"

libraryDependencies ++= Seq(
  "com.github.julien-truffaut"  %%  "monocle-core"    % libraryVersion,
  "com.github.julien-truffaut"  %%  "monocle-generic" % libraryVersion,
  "com.github.julien-truffaut"  %%  "monocle-macro"   % libraryVersion,        
  "com.github.julien-truffaut"  %%  "monocle-law"     % libraryVersion % "test" 
)

// for @Lenses macro support
addCompilerPlugin("org.scalamacros" %% "paradise" % "2.0.1" cross CrossVersion.full)
```

# Optics

-   [Lens](tut/lens.html)