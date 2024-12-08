# FETCH & AXIOS
Both are used for making HTTP request from the browser.

# Fetch
- Native Browser API to make HTTP Request [Built in Modern Browser]
- Fetch is supported by all modern browsers, not support Internet Explorer (IE).

# Axios
- Third party Library
- npm install axios
- works in all browsers including Internet Explorer 11 and below

# Promise-based 
- Both use Promises, making then asyc
- Fetch: Returns a Promise that resolves to the Response object
- Axios: Automatically resolves or rejects based on HTTP status codes

# Handling Response Data
- Fetch: To call the .json() or .text() methods on the reponse obj to parse the response data.
- Axios: Automatically parses the JSON data

# Fetch - example

```Javascript
fetch('https://api.example.com/data')
.then(response => response.json())
.then(data => console.log(data))
```

# Axios - example
```Javascript
axios.get('https://api.example.com/data')
.then(response => console.log(response.data))
```