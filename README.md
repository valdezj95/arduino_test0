# Main board basic configuration
## [Product page](https://heltec.org/project/htcc-ab01-v2/)
## [Documentation page](https://docs.heltec.cn/en/node/asr650x/htcc_ab01/index.html)
![](https://heltec.org/wp-content/uploads/2023/10/HTCC-AB01_V2-1200x767.jpg)

Board selection:

![](board_selection.png)

Basic lorawan selection:

![](board_lorawan_basic_selection.png)

For Datacake LNS LoRaWAN, go to configuration view

![](config.png)

Test values to match with programming file:

![](lora_param.png)

Payload Decoder

```javascript
function Decoder(payload, port) {

        return [
        {
            field: "DATA_TEST0",
            value: payload[0]
        },
    
        {
            field: "DATA_TEST1",
            value: payload[1]
        },    
        
        {
            field: "DATA_TEST2",
            value: payload[2]
        },   
        
     ];

} 
```
