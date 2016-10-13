# LINK-REACT

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

## Other
- [memoizerific](https://github.com/thinkloop/memoizerific/)
- [todo-app](https://github.com/thinkloop/todo-app/)

## Like it? Star It
