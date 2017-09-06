React GitHub Fork Ribbon
=============
[![npm][npm-image]][npm-url] [![Dependency Status][david-dm-image]][david-dm-url]

Pure inline style github fork ribbon on React component. The inline style css is from ["Fork me on GitHub" CSS ribbon](http://simonwhitaker.github.io/github-fork-ribbon-css/).

|         | React = 0.12 | React = 0.13  | React >= 0.14 |
| ------- | ------------ | ------------- | ------------- |
| Version | <= 0.2       | >= 0.3 < 0.5  | >= 0.5        |

## Usage

```sh
npm install react-github-fork-ribbon
```

Ex. React 15.5
```js
import React            from 'react';
import ReactDOM         from 'react-dom';
import GitHubForkRibbon from 'react-github-fork-ribbon';

const Content = () => (
  <GitHubForkRibbon href="//www.google.com"
                    target="_blank"
                    position="right">
    Fork me on GitHub
  </GitHubForkRibbon>
);

ReactDOM.render(
  <Content />,
  document.getElementById('content')
);
```

## Attribute

#### href

It would be `<a>` tag's attribute `href`

#### target

It would be `<a>` tag's attribute `target`

#### position

It has four positions.
- `left`
- `right`
- `left-bottom`
- `right-bottom`

### color

It has four color.
- `red`
- `orange`
- `black`
- `green`

## Release Notes

### Version 0.5.0 - 2017/04/11

- Drop react 0.13 support
- Support react 15.5 for preparing upgrade to react 16
- Add jest for snapshot testing

### Version 0.4.5 - 2017/03/11

- Refactor position and color set function
- Remove object-assign library
- Use storybook to help develop

### Version 0.4.4 - 2016/04/30

- Fix React 15 unitless number warning

### Version 0.4.3 - 2016/04/18

- Support React 15.0
- Browserify bundle js file for web usage.

### Version 0.4.2 - 2015/10/11

- Support React 0.14

### Version 0.4.1 - 2015/06/29

- Insert the relevant browser prefix.
  + Webkit, Moz, O, ms.

### Version 0.4.0 - 2015/06/28

- Switch to vanilla inline styles. [PR#7](https://github.com/jessy1092/react-github-fork-ribbon/pull/7)
- Update Dev-dependencies version. `babel` => 5.6.14, `browserify` => 10.2.4

### Version 0.3.0 - 2015/03/28

- Support `react` 0.13.x and `react-style` 0.5.x version
- Use ES6 feature.

### Version 0.2.0 - 2015/03/07

- Add attribute: `color`
- Transpile into vanilla js during prepublish.

### Version 0.1.0 - 2015/01/16

- Init
- Add attribute: `href`, `target`, `position`

## Contribute
[![devDependency Status][david-dm-dev-image]][david-dm-dev-url]

1. Fork it.
2. Create your feature-branch `git checkout -b your-new-feature-branch`
3. Commit your change `git commit -am 'Add new feature'`
4. Push to the branch `git push origin your-new-feature-branch`
5. Create new Pull Request with `master` branch

## License

MIT
