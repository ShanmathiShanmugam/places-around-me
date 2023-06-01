# Places Around Me
## AIM:
To develop a website to display details about the places around my house.

## Design Steps:

### Step 1:

Open up a terminal in your preffered location, and start a django project using djang-admin startproject Next setup an app inside the project folder using django-admin startapp.
### Step 2:

Once Created ,link your app to the project by adding it in the list of apps in settings.py file located inside the project folder. Add access to your host in allowed host setting and add static folders path to your settings.py file.

### Step 3:

Create a static folder and template folder and add all your required files for the project - Images .etc in your static folder. In the Template folder add your html files required for the pages.

### Stap 4:

Head to the views.py in your app folder and create required functions to render a particular page or template when requested by the client. Next go to the urls.py and route the correct view functions to each particular request as needed.

### Step 5:

Next start the server from the projects main directory using python3 manage.py runserver 0:. Now the pages can be accessed from all the routed addresses in urls.py.

## Code:
### map.html
```
<!DOCTYPE html>
<html>
    <head>
        <title>
            Image Map
        </title>
    </head>
    <body >
        <h1 align="center" >
            <font color="red" >
                    Chennai - Ashok nagar
            </font>            
        </h1>
        <h3 align="center">
        <font color="blue" face ="cursive">
            S.SHANMATHI(212222100049)
        </font>
            
        </h3>
        <center>
        <img id="Image-Maps-Com-image-maps-2023-05-31-041615" src="../images/map1.png" border="0" width="1817" height="689" orgWidth="1817" orgHeight="689" usemap="#image-maps-2023-05-31-041615" alt="" />
        <map name="image-maps-2023-05-31-041615" id="ImageMapsCom-image-maps-2023-05-31-041615">
        <area  alt="" title="home" href="home.html" shape="rect" coords="304,279,354,329" style="outline:none;" target="_self"     />
        <area  alt="" title="hospital" href="hospital.html" shape="rect" coords="42,287,92,337" style="outline:none;" target="_self"     />
        <area  alt="" title="ground" href="ground.html" shape="rect" coords="992,110,1053,169" style="outline:none;" target="_self"     />
        <area  alt="" title="school" href="school.html" shape="rect" coords="839,574,919,655" style="outline:none;" target="_self"     />
        <area  alt="" title="cafe" href="cafe.html" shape="rect" coords="40,216,120,278" style="outline:none;" target="_self"     />
        <area shape="rect" coords="1815,687,1817,689" alt="Image Map" style="outline:none;" title="Image Map" href="https://www.image-maps.com/" />
        </map>


        </center>
        <p align="center">
            <font color="maroon"  face="Comic Sans MS" >
                This Image Map shows various locations around my home.<br>
                Click the location and get information about it.
            </font>
        </p>
    </body>
</html>
```
### home.html
```
<!DOCTYPE html>
<html>
<head>
    <title>
        HOME
    </title>
</head>
<body bgcolor="pink">
<h1 align="center">
    <font color="blue" face="cursive">
        MY HOME
    </font>
</h1>
<p align="center">
    <font color="black" face="Comic Sans MS" size="24">
        <OL  TYPE="1" START="1">
            <LI>This is my home where I live happy with my family.<br></LI>     
            <LI>My mother and Father takes care of me and I have fun with my siblings and my pets.<br></LI>
            <LI>I love my home very much.<br></LI>
            <LI>When I feel stress, I used to visit my farms around my house and the nature and its beauty makes me to feel better.<br></LI>
        </OL>
    </font>


    <font color ="red" face = "cursive" size="16" > 
    "HOME IS WHERE OUR STORY BEGINS"
    </font>
</p>
</body>
</html>
```
### school.html
```
<!DOCTYPE html>
<html>
<head>
    <title>
        SCHOOL
    </title>
</head>
<body bgcolor="yellow" >
<h1 align="center">
    <font color="blue" face="cursive">
        MY SCHOOL
    </font>
</h1>
<p align="center">
    <font color="black" face="Comic Sans MS" size="24" >
        <OL  TYPE="1" START="1">
            <LI>This is my school.<br></LI>     
            <LI>This is where i studied till tenth standard.<br></LI>
            <LI>I learnt a lot and had a lot of fun.<br></LI>
            <LI>I've got many friends there .<br></LI>
        </OL>
    </font>


    <font color ="red" face = "cursive" size="16" > 
    "SCHOOL IS PLACE WHERE WE LEARN OUR FIRST LESSONS BOTH IN ACADEMIC AND IN LIFE"
    </font>
</p>
</body>
</html>
```
### hospital.html
```
<!DOCTYPE html>
<html>
<head>
    <title>
        HOSPITAL
    </title>
</head>
<body bgcolor="beige">
<h1 align="center">
    <font color="blue" face="cursive">
        HOSPITAL
    </font>
</h1>
<p align="center">
    <font color="black" face="Comic Sans MS" size="24">
        <OL  TYPE="1" START="1">
            <LI>This is a hospital near my house.<br></LI>     
            <LI>It is pretty famous in the neighourhood for its fine medical practice.<br></LI>
            <LI>We  used to visit there for any kind of medical emergency.<br></LI>
            <LI>I personally like their hospitality and the way they communicate with the patients with patience.<br></LI>
        </OL>
    </font>


    <font color ="red" face = "cursive" size="16" > 
    "HOME IS WHERE OUR STORY BEGINS"
    </font>
</p>
</body>
</html>
```
### ground.html
```
<!DOCTYPE html>
<html>
<head>
    <title>
        GROUND
    </title>
</head>
<body bgcolor="grey">
<h1 align="center">
    <font color="sky blue" face="cursive">
        GROUND
    </font>
</h1>
<p align="center">
    <font color="black" face="Comic Sans MS" size="24">
        <OL  TYPE="1" START="1">
            <LI>This is a ground near my house.<br></LI>     
            <LI>I used to play there with my friends.<br></LI>
            <LI>I've spent half of my childhood in the ground. <br></LI>
            <LI>This ground has lot of trees and greenaries <br></LI>
        </OL>
    </font>


    <font color ="pink" face = "cursive" size="16" > 
    "A PLAYGROUND IS WHERE WE FIRST FALL DOWN AND GET UP BY OURSELVES"
    </font>
</p>
</body>
</html>
```
### cafe.html
```
<!DOCTYPE html>
<html>
<head>
    <title>
        CAFE
    </title>
</head>
<body bgcolor="purple">
<h1 align="center">
    <font color="sky blue" face="cursive">
        CAFE
    </font>
</h1>
<p align="center">
    <font color="black" face="Comic Sans MS" size="24">
        <OL  TYPE="1" START="1">
            <LI>This is a cafe in my neighbourhood.<br></LI>     
            <LI>I used to hangout here with my friends often.<br></LI>
            <LI>I have lot of memories there.<br></LI>
            <LI>The burger there tastes dso good that makes me visit often.<br></LI>
        </OL>
    </font>


    <font color ="pink" face = "cursive" size="16" > 
    "CAFE IS A PLACE I LIKE A LOT"
    </font>
</p>
</body>
</html>
```

## Output:
### Client output
## home
![Screenshot (88)](https://github.com/ShanmathiShanmugam/places-around-me/assets/121243595/c7ae8a58-6fe2-4200-a4de-88555c85c036)

## school
![Screenshot (79)](https://github.com/ShanmathiShanmugam/places-around-me/assets/121243595/e15016b0-6bba-4c9f-8fbe-3920c0cbf3f8)

## hospital
![Screenshot (85)](https://github.com/ShanmathiShanmugam/places-around-me/assets/121243595/9343dab2-f645-4197-8473-1dedcf63f1f9)

## cafe
![Screenshot (82)](https://github.com/ShanmathiShanmugam/places-around-me/assets/121243595/1097fa94-35f2-4061-a5a6-972cf3bfd0d0)

## ground
![Screenshot (87)](https://github.com/ShanmathiShanmugam/places-around-me/assets/121243595/5002e25b-35ce-4f69-b40f-1ef23401a2d4)
### Server output
![Screenshot 2023-06-01 211153](https://github.com/ShanmathiShanmugam/places-around-me/assets/121243595/df70a585-cba8-4aeb-b0b6-edb3e76ca135)

### HTML validator
![Screenshot (89)](https://github.com/ShanmathiShanmugam/places-around-me/assets/121243595/5e2863c9-f642-4c37-9e50-ae499793127d)

## Result:
Hence a website has been developed to display details about places around my house.
