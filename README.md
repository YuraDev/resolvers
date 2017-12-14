
> Creating different verification chains
# Quick start

[![NPM](https://nodei.co/npm/resolvers.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/resolvers/)
## Install the package:

```bash
npm install resolvers
// or 
yarn add resolvers
```
## Create a base resolver:
```javascript
import resolvers from 'resolvers';

let base = resolvers(param => {
  console.log('base', param)
})

let isAdmin  = base.create(param => {
  console.log('isAdmin', params)
})

isAdmin('userId')
/* run
 -> base, userId
 -> isAdmin, userId
*/
```