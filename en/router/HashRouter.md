# HashRouter
HashRouter uses the hash property of location, and it listens the hash change event to respond.  

HashRouter supports one property: basename, which is used as the base path of all urls.  

>Example:  
```xml
<HashRouter basename='/center'>
  <div>
    <ul>
      <li><Link to='/home'>Home</Link></li>
    </ul>
    <div>
      <Route path='/home' component={Home}/>
    </div>
  </div>
</HashRouter>
```
>Effect  
The real path of Home component will be `/center/home`, and the Link component will lead to `/center/home`.

