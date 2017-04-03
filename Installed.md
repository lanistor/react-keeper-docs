# Install

## Node
Install React-Keeper  
```
npm install react-keeper
```

Then use as this:  

```js
import { HashRouter, Route, Link } from 'react-keeper'
// import react, Home, Host...

const App = ()=>{
  return (
    <HashRouter>
      <div>
        <ul>
          <li><Link to='/'>Home</Link></li>
          <li><Link to='/host'>Host</Link></li>
        </ul>
        <div>
          <Route path='/' components={Home}/>
          <Route path='/host' components={Host}/>
        </div>
      </div>
    </HashRouter>
  )
}
ReactDOM.render(<App/>, document.getElementById('app'))
```

## Browser
Lead into html:  
```html
<script src='react-keeper.min.js'></script>
```

Then use as this:  

```js
var HashRouter = ReactKeeper.HashRouter,
  Route = ReactKeeper.Route,
  Link = ReactKeeper.Link

var App = function(){
  return (
    <HashRouter>
      <div>
        <ul>
          <li><Link to='/'>Home</Link></li>
          <li><Link to='/host'>Host</Link></li>
        </ul>
        <div>
          <Route path='/' components={Home}/>
          <Route path='/host' components={Host}/>
        </div>
      </div>
    </HashRouter>
  )
}
ReactDOM.render(<App/>, document.getElementById('app'))
```



