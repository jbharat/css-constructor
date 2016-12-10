### CSS constructor 💄 for React components

![beta](https://img.shields.io/badge/status-beta-yellow.svg)
--

Every React component gets a javascript constructor for functional logic.

**Introducing the css constructor for styling!**

```js
import React from 'react';
import css from 'css-constructor';

export default class Hello extends React.Component {

    /* javascript constructor */
    constructor (props) {
        super(props);
    }

    /* css constructor */
    @css`
        font-size: 16px;
        text-align: center;
        color: #5AF78E;
        font-family: monospace;
    `

    render () {
        return <div>Styled text!</div>
    }
};
```

--

**Features:**

🎀 Supports real css

🔼 Attaches **inline styles** to the highest element in your component

💄 Offical library emoji

--

*Coming soon*

🔥 use props in css

🙋 classes instead of inline styles

📱 media queries support

--

#### Usage

```
npm install css-constructor --save
```

Add a `@css` block just before the `render` function (important)

Bonus: It also works with the offical emoji
```js
@💄`
  color: #FF6962;
`
```

You can start using this right away. Even though 💄 is in `BETA`, the `@css` block will always look the same.


#### How does it work?

💄 uses [ES7 class function decorators](https://github.com/wycats/javascript-decorators) on the render function.
I'll probably write a detailed post about it.

#### Inspiration

Heavily inspired from [glamor](https://github.com/threepointone/glamor), [styled-components](https://github.com/styled-components/styled-components) and [radium](https://github.com/FormidableLabs/radium)

#### Support

If you think 💄 is useful for your project, ⭐️ this repo for my motivation 🙇🏻
