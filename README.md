# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Silicon Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/titleicon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Silicon Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contact">Contact</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Silicon Private Limited, Developed by SRIHARISH.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/building2.jpeg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sata ssd.jpg"  alt="product image">
            </div>
            <div class="itemname">wd green 240 gb 2.5 inch sata III internal solid state drive</div>
            <div class="itemprice">Price: Rs.2300.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/optical.jpg"  alt="product image">
            </div>
            <div class="itemname">optical sensor</div>
            <div class="itemprice">Price: Rs.4150.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/wireless network.jpg"  alt="product image">
            </div>
            <div class="itemname">wireless network</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/switch.jpg"  alt="product image">
            </div>
            <div class="itemname">switch</div>
            <div class="itemprice">Price: Rs.50.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/silicon battery.jpg"  alt="product image">
            </div>
            <div class="itemname"> silicon battery</div>
            <div class="itemprice">Price: Rs.50.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/silicon michrochip.jpg"  alt="product image">
            </div>
            <div class="itemname"> siicon michrochip</div>
            <div class="itemprice">Price: Rs.1560.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/watch.jpg"  alt="product image">
            </div>
            <div class="itemname">silicon watch</div>
            <div class="itemprice">Price: Rs.560.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/silicon gun.jpg"  alt="product image">
            </div>
            <div class="itemname">siicon gun</div>
            <div class="itemprice">Price: Rs.120.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/silicon wafer.jpg"  alt="product image">
            </div>
            <div class="itemname">siicon wafer</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/silicon wire.jpg"  alt="product image">
            </div>
            <div class="itemname">siicon wire</div>
            <div class="itemprice">Price: Rs.20.00 </div>
        </div>
    </div>
    </div>
{% endblock %}    
```
# people.html

```
{% extends "website/base.html" %}

{% block content %}
<div class="productcontent">    
    <h1>BUSINESS MAN</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/photo1.jpg" alt="product image">
            </div>
            <div class="itemname">sundar pichai</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/photo 2.jpg"  alt="product image">
            </div>
            <div class="itemname">jack ma</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/photo3.jpg"  alt="product image">
            </div>
            <div class="itemname">steve jobs</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/photo4.jpg"  alt="product image">
            </div>
            <div class="itemname">mukesh ambony</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/photo5.jpg"  alt="product image">
            </div>
            <div class="itemname">bernand arnault</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/photo6.jpg"  alt="product image">
            </div>
            <div class="itemname">warren buffet</div>
        </div>

    </div>
    </div>
{% endblock %}        
```
# contact.html

```
{% extends "website/base.html" %}

{% block content %}
<h1>CONTACT DETAILS:</h1> 
<h2>SILICON GROUP OF COMPANIES<h2>
<h3>#54th Avenue,Adyar,<h3>
     <h3>BANGALORE<h3>
   <h3>email:siliconSOC9876@gmail.com<h3>
   <h3>mobile:6598604XYZ<h3>
   <h3>land-line:044-765478<h3>
   {% endblock %}

```
###
## OUTPUT:
![output](./static/img/Screenshot(18).png)

![output](./static/img/Screenshot1.png)

![output](./static/img/Screenshot20.png)

![output](./static/img/Screenshot21.png)

![output](./static/img/Screenshot22.png)

## CODE VALIDATION REPORT:
![output](./static/img/Screenshot23.png)

![output](./static/img/Screenshot24.png)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://sriharish.student.saveetha.in:8000/. HTML code is validated.