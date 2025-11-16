# This is my repository
## My name is Nastia

**This text will be bold**
*This text will be bold*

This is Unordered list:
* Item 1
* Item 2
  *  Item 2a
    ```javascript
    let str ='this is js code';
  
!.[this is img]<img width="2121" height="1193" alt="image" src="https://github.com/user-attachments/assets/efc1011b-4395-4b53-ad96-703ae9644a5e" />

const kantoPokemonsRequest = new XMLHttpRequest();
kantoPokemonsRequest.open('GET','https://pokeapi.co/api/v2/pokemon?limit=127');
kantoPokemonsRequest.responseType = 'json';
kantoPokemonsRequest.send();
kantoPokemonsRequest.onload = function() {
    kantoPokemonsRequest.response.results.forEach(pokemon => {
        let promise = new Promise(function(resolve, reject) {
            let xhr = new XMLHttpRequest();
            xhr.open('GET', pokemon.url);
            xhr.responseType = 'json';
            xhr.send();
            xhr.onload = function() {
                if(xhr.status == 200) {
                    resolve(xhr.response);
                }
                else {
                    reject(xhr.statusText)
                }
            }
            xhr.onerror = function() {
                reject(xhr.statusText);
            }
        });
    });
