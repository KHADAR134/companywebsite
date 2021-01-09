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
        <div class="menuitem"><a>People</a></div>
        <div class="menuitem"><a>Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Silicon Private Limited, Developed by Obed Otto.
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
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications. Some of Silicon's core technologies and products include:
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
            <img src="/static/img/amegon.jpg"  alt="product image">
            </div>
            <div class="itemname">AMEGON 4GB DDR3 </div>
            <div class="itemprice">Price: Rs.1500.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/i3 processor.jpg"  alt="product image">
            </div>
            <div class="itemname">Intel Core i3-9100F 9th Gen</div>
            <div class="itemprice">Price: Rs.7000.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/kingston ssd.jpg"  alt="product image">
            </div>
            <div class="itemname">Kingston SSDNow A400 240GB</div>
            <div class="itemprice">Price: Rs.2700.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/Crucial.jpg"  alt="product image">
            </div>
            <div class="itemname">Crucial BX500 480GB 3D NAND SATA 2.5-inch SSD</div>
            <div class="itemprice">Price: Rs.4300.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/corsair.jpg"  alt="product image">
            </div>
            <div class="itemname">Corsair CV650</div>
            <div class="itemprice">Price: Rs.5500.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/corsair RM.jpg"  alt="product image">
            </div>
            <div class="itemname">Corsair RM650</div>
            <div class="itemprice">Price: Rs.10500.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/antec.jpg"  alt="product image">
            </div>
            <div class="itemname">Antec NeoEco 650M</div>
            <div class="itemprice">Price: Rs.4600.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/Dlink.jpg"  alt="product image">
            </div>
            <div class="itemname">D-Link DSL-2730U Wireless-N 150 ADSL2+ 4-Port Router</div>
            <div class="itemprice">Price: Rs.1000.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/Tplink.jpg"  alt="product image">
            </div>
            <div class="itemname">TP-LINK TD-W8961N Wireless</div>
            <div class="itemprice">Price: Rs.1200.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/tplink ac1300.jpg"  alt="product image">
            </div>
            <div class="itemname"> TP-Link Archer T3U AC1300 Mini Wireless MU-MIMO USB Adapter</div>
            <div class="itemprice">Price: Rs.1500.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
## people.html:
```
{% extends "website/base.html" %}

{% block content %}
        <div class="peoplecontent">    
    <h1>OUR EXECUTIVE LEADERSHIP TEAM</h1>
    <div class="peoplelists">
        <div class="peoplelist"> 
            <div class="peopleimage">
            <img src="/static/img/s1.jpg" alt="people image" width="300" height="300">
            </div>
            <div class="peoplename">
                <h2>FAZAL</h2></div>
            <div class="peoplepost">
                <h3>(C.E.O)</h3></div>
        </div>
        <div class="peoplelists">
        <div class="peoplelist"> 
            <div class="itemimage">
            <img src="/static/img/s3.jpg" alt="people image" width="300" height="300">
            </div>
            <div class="peoplename">
                <h2>Martin</h2></div>
            <div class="peoplepost">
                <h3>(SENIOR VICE PRESIDENT)</h3></div>
        </div>
         <div class="peoplelists">
        <div class="peoplelist"> 
            <div class="itemimage">
            <img src="/static/img/s5.jpg" alt="product image" width="300" height="300">
            </div>
            <div class="peoplename">
                <h2>JONATHAN IVE</h2></div>
            <div class="peoplepost">
                <h3>(CHEIF DESIGNER OFFICER)</h3></div>
        </div>
         <div class="peoplelists">
        <div class="peoplelist"> 
            <div class="itemimage">
            <img src="/static/img/s6.jpg" alt="product image" width="300" height="300" >
            </div>
            <div class="itemname">
                <h2>JEFF WILLIAMS</h2></div>
            <div class="itemprice">
                <h3>(CHEIF OPERATING OFFICER)</h3></div>
        </div>
         <div class="peoplelists">
        <div class="peoplelist"> 
            <div class="itemimage">
            <img src="/static/img/s7.jpg" alt="product image" width="300" height="300">
            </div>
            <div class="peoplename">
                <h2>DAVID</h2></div>
            <div class="peoplepost">
                <h3>(VICE PRESIDENT MARKETING)</h3></div>
        </div>
         <div class="peoplelists">
        <div class="peoplelist"> 
            <div class="itemimage">
            <img src="/static/img/s8.jpg" alt="product image" width="300" height="300">
            </div>
            <div class="itemname">
                <h2>DAN</h2></div>
            <div class="itemprice">
                <h3>(VICE PRESIDENT HARDWARE TECHNOLOGY)</h3></div>
        </div>
{% endblock  %}
```
## contactus.html:
```
{% extends "website/base.html" %}
{% block content %}

<div class="content1">
    <h1 class="contactcenter">
        CONTACT US</h1>
    <h2 class="contactcenter">
        CONTACT ADDRESS:Central Province,Malaz Area,Salahuddin Al-Ayoubi Street,Albawardi Building, P.O.Box 68,Riyadh
        11411, Saudi Arabia
        <br>
        EMAIL:fazal87@gmail.com
        <br>
        MOBILE:+966598712543
    </h2>
</div>
{% endblock  %}

```    

## OUTPUT:
![output](./static/img/output1.jpg)

![output](./static/img/output2.jpg)

![output](./static/img/output3.jpg)

![output](./static/img/output4.jpg)

![output](./static/img/output5.jpg)

![output](./static/img/output6.jpg)

![output](./static/img/output7.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/report1.jpg)

![output](./static/img/report2.jpg)

![output](./static/img/report3.jpg)

![output](./static/img/report4.jpg)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://khadar.student.saveetha.in:8000/. HTML code is validated.