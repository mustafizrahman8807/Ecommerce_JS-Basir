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
