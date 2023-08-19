# Request-API

##Javascript Promise Code

```javascript

const url = 'https://api.coindesk.com/v1/bpi/currentprice.json';
            const request = new XMLHttpRequest();
            request.open('GET', url);
            request.onreadystatechange = function(){
                console.log(request.readyState);
                if(request.readyState === 4){ 
                const da = this.responseText;
                console.log(da);
                    const data  = JSON.parse(this.responseText);
                    console.log(data);
                    console.log(data.chartName);
                 }
            }
            console.log("DONES");
            request.send();

```
