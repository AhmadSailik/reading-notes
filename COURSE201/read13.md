- **HTML5:**it's allow for pages to store named key/value pairs locally
- you can check for HTML5 Storage by
    - `function supports_html5_storage() {`
`try {`
`return 'localStorage' in window && window['localStorage'] !== null;`
`} catch (e) {`
` return false;`
`}`
`}`

    - `if (Modernizr.localstorage) {`
`// window.localStorage is available!`
`} else {`
`// no native support for HTML5 storage :(`
`// maybe try dojox.storage or a third-party solution`
`}`
- any type of data is store as string
- limitations in current browsers 
    - 5 megabytes
    - QUOTA_EXCEEDED_ERR
    - No
