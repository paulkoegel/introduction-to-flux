class: background-grey flux-title

# Flux

[https://facebook.github.io/flux](https://facebook.github.io/flux)

.flux-logo[![Flux logo](images/flux-logo.svg)]

---

background-image: url(images/flux-diagram.png)

---

**Actions**: an object literal containing new data and a specific type, allowing Stores to discern whether it is relevant to their domain.

**Dispatcher**: a registry of callbacks that, by way of the callbacks, distributes a payload (an Action) to the registrants (the Stores). It has no intelligence of its own. All intelligence is in the Stores.

**Stores**: a domain model which registers itself with the Dispatcher and emits a 'change' event whenever a change in its state occurs.

**Utils**: libraries of pure functions that can be easily shared across different modules.

---

**Controller-views**: view components near the root of the component tree. They listen for 'change' events in stores and respond to this event by retrieving new data through the store's exposed getter methods and passing it to their children. The only difference between Controller-views and Views is this listening functionality.

**Views**: stateless children of the controller-view components, receiving and passing along data, much like pure functions. Views and Controller-views are most often implemented with React, as it provides the ability to re-render at will with very little performance loss.


---

## Dan Abramov's Flux Cheat Sheet

![Dan Abramov's Flux Cheat Sheet](images/dan-abramovs-notes.png)

---


## Links - Part 1

+ Best presentation I know: ["Flux - Those who forget the past..."](https://speakerdeck.com/jmorrell/jsconf-uy-flux-those-who-forget-the-past-dot-dot-dot-1)
+ Video workshop covering Flux: [React.js Workshop with Ryan Florence](https://frontendmasters.com/workshops/react-js/)
+ [https://stackoverflow.com/questions/27264487/from-angularjs-to-flux-the-react-way/27267083#27267083](https://stackoverflow.com/questions/27264487/from-angularjs-to-flux-the-react-way/27267083#27267083)
+ [https://medium.com/brigade-engineering/what-is-the-flux-application-architecture-b57ebca85b9e](https://medium.com/brigade-engineering/what-is-the-flux-application-architecture-b57ebca85b9e)
+ [https://medium.com/@goatslacker/principles-of-flux-ea872bc20772](https://medium.com/@goatslacker/principles-of-flux-ea872bc20772)

---

## Links - Part 2

comparison of Flux implementations:
+ [http://pixelhunter.me/post/110248593059/flux-solutions-compared-by-example](http://pixelhunter.me/post/110248593059/flux-solutions-compared-by-example)

global app state:
+ [https://gist.github.com/paulwittmann/9880692](https://gist.github.com/paulwittmann/9880692)
+ [http://blog.circleci.com/local-state-global-concerns](http://blog.circleci.com/local-state-global-concerns)
