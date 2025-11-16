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
  
!.[this is img]https://www.cdc.gov/healthy-pets/media/images/2024/04/GettyImages-598175960-cute-dog-headshot.jpg
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
