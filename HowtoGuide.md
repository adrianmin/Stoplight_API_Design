

---
stoplight-id: 8o46ywa3didi0
---

# How To Guide

If you are wondering how to use the API calls within your code base, here is a list of ReactJS based functions that you can tailor to your needs

## How to get all auto parts
```
#Get list of parts
async function GetAutoParts() {
    return fetch('http://api.se.autoparts.com/parts',{
        method: 'POST',
        header: {
            'Content-Type': 'application/json',
            'authorization': your_autoparts_token,
        },
        body: JSON.stringify()
    }).then(data => data.json())
}
```


## How to get an auto part by part number

```
#Get a part by part nummber/id
async function GetAutoPartById(props) {
    return fetch('http://api.se.autoparts.com/part/{props.part.id}',{
        method: 'POST',
        header: {
            'Content-Type': 'application/json',
            'authorization': your_autoparts_token,
        },
        body: JSON.stringify()
    }).then(data => data.json())
}
```


## How to get delete an auto part by part number
Information on content category 3

## How to get all auto part orders

Information on content category 4

## How to get an auto part order by order number

Information on content category 5

## How to create a new auto part order

Information on content category 6
