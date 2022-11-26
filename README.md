# create-npm-package-and-link-local
1. create new Folder "mkdir my-package"
    ```D:\Desktop>mkdir my-package```
2. run ```npm init -y``` inside my-package
    D:\Desktop\my-package>npm init -y
3. The ```npm init -y```command creat package.json and point to index.js as a main in package.json
4. create index.js inside the "my-package" folder
    ```sh
    console.log('muliplication package');
    const multiplication =  (x,y) => {
      return x*y;
    }
    module.export = multiplication;
    ```
6. Then run link comma
7. create 'my-package' folder inside the npm-own-package
