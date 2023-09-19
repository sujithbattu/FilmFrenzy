# FilmFrenzy

An immersive application built entirely in SwiftUI, FilmFrenzy showcases movies leveraging the MovieDB API. Designed to demonstrate the capabilities of SwiftUI and Combine, it is a continuous effort to push the boundaries of what's achievable with SwiftUI without reverting to UIKit.

## Core Principles
- **Real-world Application**: The aim is to demonstrate how a practical application can be built using only SwiftUI, evolving with each update and addition to the framework.
- **Pure SwiftUI**: No reliance on UIView/UIViewController representables, a testament to the depth of SwiftUI's capabilities.

## Architecture

FilmFrenzy embraces a data flow inspired by the Flux segment of [Redux](https://redux.js.org/). The state, embedded as an [ObservableObject](https://developer.apple.com/documentation/combine/observableobject), publishes changes in response to dispatched actions. By injecting this state as an environment object at the root, it's effortlessly accessible application-wide.

SwiftUI intelligently handles state changes, performing diffing during the render phase. The efficiency of SwiftUI hinges on the intricacy of the view hierarchy, sidelining the complexity of the object graph.

## Platforms

FilmFrenzy is adaptable across iPhone, iPad, and macOS, demonstrating versatility and expansive reach.

