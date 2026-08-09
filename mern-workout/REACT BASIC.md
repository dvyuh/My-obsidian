
need to know when a state changes ui is updated EVERY SINGLE TIME

every component is automatically updated and re rendered to the screen

ie. state change--- code is rerunned everything in the code but the 

-- 
basiclally we need this
```
import { useState } from "react";

  
function Home(){
  

const [searchQuery, setSearchQuery] = useState("");
```

we need to define the state as if we dont and it changes the change wouldnt be noted.


## Page routing

 npm install react-router-dom

```
import { createRoot } from 'react-dom/client'

import {BrowserRouter} from "react-router-dom"

import './index.css'

import App from './App.jsx'

  

createRoot(document.getElementById('root')).render(

<StrictMode>

<BrowserRouter>

<App />

</BrowserRouter>

</StrictMode>,

)
```

importing browser router this is for yk the search bar going name/second
name/first

this helps in moving from one page to another

---
## FETCHING SHIT AND USE_EFFECT

use effect allows you to add side effect to your functions or the components and define when they should run

