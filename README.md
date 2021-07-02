# Ecommerce_JS-Basir

**1. Create Folder Structure**

    i. create root folder as jsamazona
    ii. add frontend and backend folder
    iii. create src folder in frontend
    iv. create index.html with heading jsamazona in src
    v. run npm init in frontend folder
    vi. npm install live-server
    vii. add start command as live-server src --verbose
    viii. run npm start
    ix. check result
    
**2. Design Website**

    i. create style.css
    ii. link style.css to index.html
    iii. create div.grid-container
    iv. create header, main and footer
    v. style html, body
    vi. style grid-container, header, main and footer
    
    *3. Create Static Home Screen**

    i. create ul.products
    ii. create li
    iii. create div.product 
    iv. add .product-image, .product-name, .product-brand, .product-price
    v. style ul.products and internal divs
    vi. duplicate 2 times to show 3 products
    
**4. Render Dynamic Home Screen**
 
    i. create data.js
    ii. export an array of 6 products
    iii. create screens/HomeScreen.js
    iv. export HomeScreen as an object with render() method
    v. implement render()
    vi. import data.js
    vii. return products mapped to lis inside an ul
    viii. create app.js
    ix. link it to index.html as module
    x. set main id to main-container
    xi. create router() function
    xii. set main_container innerHTML to HomeScreen.render()
    xiii. set load event of window to router() function
    
*5. Build Url Router**

    i. create routes as route:screen object for home screen
    ii. create utils.js
    iii. export parseRequestURL()
    iv. set url as hash address split by slash
    v. return resource, id and verb of url
    vi. update router()
    vii. set request as parseRequestURL()
    viii. build parsedUrl and compare with routes
    ix. if route exists render it, else render Error404
    x. create screens/Error404.js and render error message  
 
    
**6. Create Node.JS Server**

    i. run npm init in root jsamazona folder
    ii. npm install express
    iii. create server.js
    iv. add start command as node backend/server.js
    v. require express
    vi. move data.js from frontend to backend
    vii. create route for /api/products
    viii. return products in data.js
    ix. run npm start

**7. Load Products From Backend**

    i. edit HomeScreen.js
    ii. make render async
    iii. fetch products from '/api/products' in render()
    iv. make router() async and call await HomeScreen.render()
    v. use cors on backend    
    vi. check the result
    
**8. Add Webpack**

    i. cd frontend
    ii. npm install -D webpack webpack-cli webpack-dev-server
    iii. npm uninstall live-server
    iv. "start": "webpack-dev-server --mode development --watch-content-base --open"
    v. move index.html, style.css and images to frontend folder
    vi. rename app.js to index.js
    vii. update index.html
    viii. add script main.js before body tag
    ix. npm start
    x. npm install axios
    xi. change fetch to axios in HomeScreen
