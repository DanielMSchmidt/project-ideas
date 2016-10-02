# Ideas

This are all ideas of programming related stuff, that I might do in my free time. Just a reminder for me, but if you need a project you are free to implement something from his list. It currently includes

- [Projects](https://github.com/DanielMSchmidt/project-ideas/blob/master/README.md#projects)
- [Blog Posts](https://github.com/DanielMSchmidt/project-ideas/blob/master/README.md#blog-posts)

## Projects
Some project ideas I would like to do in my spare time, not ranked anyhow. Please let me know if you are working on a similar problem and if you need help with it.

### [Hub](https://github.com/github/hub) for Stash

Most important features: 

- `git pull-request`
- `git create`
- `git browse`
- `git checkout`

### Feature Center

Write a Client side module which gets initialized with

- a server URL
- a unique ID for this client (on native e.g. UUID)

and then have an API like this

```javascript
import featureCenter from 'feature-center';

const features = new featureCenter({
  serverUrl: 'http://myAwesomeServer.cool',
  uniqueDeviceId: getUniqueId(),
  cacheTime: 24 * 60 * 60 * 1000, // optional (in ms)
  prefetch: ['myAwesomeFeature'] // 
});

// myAwesomeFeature may not have a space, should check this
features.mayIDoThis('myAwesomeFeature').then(function() {
  // insert awesome code here
}
```

The server should have a `api?feature=<featureName>` endpoint which returns `true` or `false`. The API should cache this for a period of time, which may be defined in the constructor. Another endpoint would be a post to `api` with a query object which looks like this: 

```json
{
  "prefetch": ["myAwesomeFeatureOne", "myAwesomeFeatureTwo"]
}
```

and returns

```json
{
  "myAwesomeFeatureOne": true,
  "myAwesomeFeatureTwo": false,
}
```

It should also provide a dashboard in which a new String may be added. There should be a default set in which each dashboard may be set to `true` or `false` and a search field for a unique device ID in which one may be selected and may select that individually.

Additionally a decorator for react components would be cool: 

```javascript
@feature('myAwesomeComponent')
class HelloMessage extends React.Component {
  render() {
    return <div>Hello {this.props.name}</div>;
  }
}
```

So that he component is only rendered if the feature is 


### Competitive Dancing Rating

Build the DTV voting system as a react native app


### RemindMe Github Bot

A github Bot, which lets you write a message like this: `@remindMeBot user/project#issuenr` and answers `I will remind you when user/project#issuenr is closed`. It should wait for `user/project#issuenr` to be closed and then comment the current issue again.

### Choreography Builder

Relay / Graphql App, that lets you build you choreography and add notes to the entries.

### React Native min-height / max-height

Is listed as Product Pain, may be implemented by measuring after re-render and setting the height accordingly. Could be expensive, so choose as seldom as possible (as disclaimer)

### React Native Responsive Stylsheets

Wrapper for Stylesheets which has `mobile`, `tablet`, `horizontal`, `vertical` prefixes and applies media queries like, through returning different styles from the stylesheet constructor


## Blog Posts

### How to pitch React Native

Series about how to pitch React Native to

- [X] [Developers](https://medium.com/@dschmidt1992/how-to-pitch-react-native-to-developers-dcf092cb4614#.s2xiz7nvz)
- [X] Team Leads
- [ ] Designers
- [ ] Top Level Executives

### Reindex + React Native + Relay

Introduction => boilerplate code

### I <3 ES6 (Advanced stuff)

Write about easy moduling, generators and proxies

### React-Native Module Generator

Present my react-native module generator and talk about the reason to write it and the roadmap.

### Show how to use redial with redux

Maybe on RN, just because fun. [Redial](https://github.com/markdalgleish/redial)

### First example with [React TVML](https://github.com/ramitos/react-tvml)

Build a small apple tv app, will sure be fun

### React-Native iOS View Lib

How to use a iOS lib with a view component as rn module

### Electron vs. RN Desktop 

Compare both in terms of usability, stability, speed of development, etc

### React Native rendering performance

When to use which technique (idleTime, animationFrame, interactionHandle)

### Build a demo application with Shoutem UI toolkit

Maybe something E-Commerce like or a list of podcast or sth similar. [Shoutem](https://shoutem.github.io/ui/)

## Archive

Blog posts or projects that are actually done.

### Best News Resource

Podcasts, Blogs, etc, all RN / JS related

### [I <3 ES6 (simple stuff)](https://medium.com/@dschmidt1992/the-benefit-of-transpiling-es2015-e84ad0fde0c1#.q3qp5j4ui)

Write about deconstructing and arrow functions (how they increase verbosity)

### [React-Dom + Server Side Rendering: How to deal with auto fill ins](https://medium.com/@dschmidt1992/auto-fill-with-redux-forms-9b51ad8ef962#.9s5ptjx9i)
Find a solution and post it (most likely set state on component will mount, [for chrome at least](http://stackoverflow.com/questions/11708092/detecting-browser-autofill))
