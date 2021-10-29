# React Tiktok Helper

This package contains "Tiktok Pixel" for tiktok ads. Already used in the Next.js project. it has been compailed using Babel.js, so it can run on old browsers.

## Install

```bash
  npm i react-tiktok-helper --save
```

## Example

I recommend that tiktok.config() is called in the react context or it should be in the \_app.js file.

```javascript
import React, { useEffect } from 'react';
import tiktok from 'react-tiktok-helper';


function App() {

    function handleClick(){
        tiktok.event('Purchase', {
          content_id: '123',
          content_type: 'product',
          price: 666,
          quantity: 1,
          currency: 'IDR',
        });
    }


    useEffect(() => {
        tiktok.config(`${YOUR_EVENT_ID}`);
    }, []);

	return (
		// .../
	);
}

```

## Documentation

-   [Parameters and Standard Events Tiktok](https://ads.tiktok.com/help/article?aid=10028)

## Authors

-   [@firmnardians](https://github.com/firmnardians)
