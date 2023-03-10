# Plotly.js for Interactive SVG Data Visualizations

__tommy teaches tommy__ (_and anyone else who cares to read all this_) about software development and coding with the [Plotly.js](https://plotly.com/javascript/) JavaScript Library variant of the Open-Source __Plotly__ data graphing library.

`plotly.js` is not the only such library for abstracting WebGL and the `<canvas>` element, but it's an arguably interesting, helpful, and mostly simple-to-use library for interactive 2D Graphics without the complexity of 3D mathematics (if that's appealing to you or your project goals).

Note that some of these examples I'm providing here will be self-contained (and possibly modified) variants of things I have up-and-running on my personal website [`tommypkeane.com`](https://www.tommypkeane.com); and since I've kept the source repo for that site private, I'm sharing things here to make them easier to find/review. You can always inspect the source code of my site, but this is arguably much better.

<!-- MarkdownTOC -->

- [Setup](#setup)
- [Running the Code](#running-the-code)
- [What's this "tommy teaches tommy" thing all about?](#whats-this-tommy-teaches-tommy-thing-all-about)
- [License](#license)
- [References](#references)

<!-- /MarkdownTOC -->

<a id="setup"></a>
## Setup

- `nvm install` will make sure that the correct version of Node.js is available
- `direnv allow` will establish a local environment using the correct version of Node.js

You can confirm that the above worked by comparing the output of these two commands:

- `node --version`
- `cat ./.nvmrc`

<a id="running-the-code"></a>
## Running the Code

Unlike the pure JavaScript examples, the usage of `plotly.js` actually requires a Web Browser, due to the way that the Library has been written 😭😭😭 ... so we need to actually run a local webserver and serve-up a local website through HTML, CSS, and JavaScript in order to most easily and directly see the results of the `plotly.js` examples that we're providing here.

Technically speaking, there are other ways to do this, including the use of NPM and registering with a `plotly.js` API Key, but we'd still need to use something like `browserify` to put it all together and serve-up the code, or go all in on an Application framework like `electron`.

Personally, I don't wanna do all that just for these examples, because that's a whole other thing, and all I'm trying to get at here is actually to look at how `plotly.js`, itself, actually works and how we can use it to create different kinds of interactive plots and graphs.

Ok, so with all that out of the way ... how do we run these examples? Basically, if you run these commands, you'll install and then start the local webserver, and then you simply open the provided `localhost` URL in your contemporary Web-Browser application of choice, and you should be greeted with a webpage that allows you to navigate to see each example.

Note that if you change any of the code, you will have to refresh your browser (potentially doing a hard refresh to clear any cached data) to pull in the changed code and see the updated renderings.

1. `nvm install` (optional, first time only)
1. `direnv allow` (first time only)
1. `npm install`
1. `npm run start` (see `package.json`)

<a id="whats-this-tommy-teaches-tommy-thing-all-about"></a>
## What's this "tommy teaches tommy" thing all about?

_"What's in a name?"_

You can see a rambly explanation [here at my personal website](https://tommypkeane.com/about-tommy/tommy-teaches-tommy.html); but, in short:

I'm just trying to say that I'm writing out what I think is helpful/interesting to me, and I'm sharing it in case it's helpful to anyone else, but please know that I'm ___not___ trying to talk _down_ to anyone :smile: (except maybe myself :ghost:).

<a id="license"></a>
## License

Copyright (c) 2023, Tommy P. Keane (https://www.tommypkeane.com)

See the [LICENSE](./LICENSE) file for details.

<a id="references"></a>
## References

- https://www.npmjs.com/package/http-server
- https://github.com/plotly/plotly.js/issues/6483
