# Router
Keeper provides three Router components: HashRouter, BrowserRouter, MemoryRouter, they have the same basic usage:  
```js
import { BrowserRouter, Route } from 'react-keeper'
// import react, Home, Host...

const App = ()=>{
  return (
    <BrowserRouter>
      <div>
        <Route path='/' components={Home}/>
        <Route path='/host' components={Host}/>
      </div>
    </BrowserRouter>
  )
}
ReactDOM.render(<App/>, document.getElementById('app'))
```

Advanced, they fit diffrent usage scences, and they have different properties defined.
