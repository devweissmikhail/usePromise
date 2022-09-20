# usePromise
usePromise - React Hook

### Usage example

```javascript
import React, { useEffect } from 'react';
import { usePromise } from './usePromise';


export default const app = () => {

	const [initPromise, initResolve, initReject] = usePromise();

	useEffect(() => {

		setTimeout(initResolve, 2000);

		initPromise.then(() => {
			console.log('test promise');
		});

	}, []);

}
```
