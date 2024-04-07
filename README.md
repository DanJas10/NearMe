# Ex04 Places Around Me
## Date: 07.04.2024

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Map</title>
</head>
<body>

    <img src="img.jpg" width="800" height="436" usemap="#mapNew" onmousemove="coordinate(event)">

    <map name="mapNew">
        <area shape="RECT" coords="280,230,430,240" href="https://www.indusind.com/" title="Indusind bank">
        <area shape="RECT" coords="450,220,530,260" href="https://www.kotak.com/" title="Kotak Mahindra bank">
        <area shape="RECT" coords="430,350,560,380" href="https://www.icicibank.com/" title="ICICI bank">
    </map>

    <br>

    X-coordinate <input type="text" id="X"> <br>
    Y-coordinate <input type="text" id="Y">

<script>
    function coordinate(event) {
        let x = event.clientX;
        let y = event.clientY;
        document.getElementById("X").value = x;
        document.getElementById("Y").value = y;
    } 
</script>

</body>
</html>
```

## OUTPUT

![Alt text](img.jpg)





## RESULT
The program for implementing image maps using HTML is executed successfully.
