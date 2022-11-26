# create-npm-package-and-link-local
1. create new Folder "mkdir my-package"
    ```D:\Desktop\npm-own-package>mkdir my-package```
2. run ```npm init -y``` inside my-package
    D:\Desktop\npm-own-package\my-package>npm init -y
3. The ```npm init -y```command creat package.json and point to index.js as a main in package.json
4. create index.js inside the "my-package" folder. add below code in to the index.js
    ```sh
    console.log('muliplication package');
    const multiplication =  (x,y) => {
      return x*y;
    }
    module.export = multiplication;
    ```
6. Then run link commad 
    ```D:\Destop\npm-own-package\my-package>npm link```
8. create 'my-app' folder inside the npm-own-package
    ```D:\Desktop\npm-own-package>mkdir my-app```
9. create index.js inside the my-app and add below code
    ```sh
    const {multiplication} = require('my-package');
    console.log('Mulitiplicaiton Answer', multiplication(5,2));
    ```
 10. After careating the index.js, link the my-packge to our applicaiton
        ```npm linkn my-package```
 11. Then run the applicaiton ```D:\Destop\npm-own-package\my-app>node index.js```
