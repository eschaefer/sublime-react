# sublime-react

Snippets and syntax highlighting for React.js / JSX.

*Updated for ES6 syntax*

![alt tag](https://raw.github.com/jgebhardt/sublime-react/master/docs/img/sr-rcc-out.gif)

## Installation

Install the React package via Sublime's Package Manager

You will need the Sublime [Package Manager](https://sublime.wbond.net/installation).

- Open the command palette: `⌘+shift+p` on MacOS/Linux, `ctrl+shift+p` on Windows

- type `package`, select `Package Control: Add Repository`

- paste in the address of this Github URL: `https://github.com/eschaefer/sublime-react`

- Again open the command palette, type `install`, select `Package Control: Install Package`

- type `React`, select `sublime-react`, note the source is this Github repo, and select that package.


## Usage

### Syntax highlighting

JSX syntax highlighting provided by [yungsters/sublime](https://github.com/yungsters/sublime)

![JSX syntax highlighting](https://raw.github.com/jgebhardt/sublime-react/master/docs/img/sr-jsx-out.gif)

To default to JSX highlighting, open a `.js` or `.jsx` file, then select from the main menu:

`View` > `Syntax` > `Open all with current extension as...` > `ReactJS` > `JavaScript (JSX)`

JSX is fully compatible with plain JavaScript.

### Snippets

It's easy! Simply activate snippets by typing a mnemonic followed by TAB.

![alt tag](https://raw.github.com/jgebhardt/sublime-react/master/docs/img/sr-snippets-out.gif)

Snippets are available for both JSX and CJSX ([React CoffeeScript](https://github.com/jsdf/coffee-react-transform)).

#### Documentation of available snippets (JSX):

```
    cdm→  componentDidMount() { ... }

   cdup→  componentDidUpdate(pp, ps) { ... }

     cs→  var cx = React.addons.classSet;

    cwm→  componentWillMount() { ... }

    cwr→  componentWillReceiveProps(np) { ... }

    cwu→  componentWillUpdate(np, ns) { ... }

   cwun→  componentWillUnmount() { ... }

     cx→  cx({ ... })

    fup→  forceUpdate(...)

    gdp→  getDefaultProps() { return {...} }

    gis→  getInitialState() { return {...} }

    ism→  isMounted()

    jsx→  /** @jsx */

  props→  this.props.

     pt→  propTypes { ... }

    rcc→  component skeleton

    ren→  render() { return ... }

    scu→  shouldComponentUpdate(np, ns) { ... }

    sst→  setState({ ... })

  state→  this.state.

    trp→  transferPropsTo( ... )

```

## Contributing

### Rebuilding the docs

After making changes to snippet files, run `npm install && npm run build-docs` to automatically generate this document from source.

### Updating JSX syntax highlighting

To pull in updates from yungsters/sublime, run:

`git subtree pull --prefix syntax/jsx https://github.com/yungsters/sublime.git master --squash`

### Contributor License Agreement

Contributions are very welcome, but we ask that you please fill out our [CLA](https://code.facebook.com/cla) in order for us to accept your pull request.

