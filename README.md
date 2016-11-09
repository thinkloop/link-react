# Link (React)

A generalized link `<a>` component that allows client-side navigation, while ignoring:

- shift-clicking
- alt-clicking
- ctrl-clicking
- non-left clicking
- `target` attribute
- `mailto` href

## Install

```
npm install link-react --save
```

React itself is a peer dependency and not included, it is the responsibility of the implementing app to provide a reference to `React`.

## Use

```
import React from 'react';
import Link from 'link-react';

export default (p) => (
	<nav>
		<Link href={ p.homeLink.href } onClick={ p.homeLink.onClick }>{ p.homeLink.label }</Link>
		<Link href={ p.aboutLink.href } onClick={ p.aboutLink.onClick }>{ p.aboutLink.label }</Link>
	</nav>
);

```

## License

Released under an MIT license.

## Related
- [state-driven routing](https://github.com/thinkloop/state-driven-routing): Full-featured, dependency-free, dsl-free, state-driven routing.


## Other
- [extreme decoupling todo app](https://github.com/thinkloop/todo-app/): Example todo app of extreme decoupling of react, redux and selectors
- [memoizerific](https://github.com/thinkloop/memoizerific/): Fast, small, efficient JavaScript memoization to memoize JS functions

#### Like it? Star It
