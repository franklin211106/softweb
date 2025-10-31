# Ex.07 Restuarant Website
## Date:31-10-25

## AIM:
To develop a static Resturant website to display the menu and services provided by the resturant.

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

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```html
<!DOCTYPE html>
<html lang="en"> 
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>RED DRAGON</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body, html { width: 10; height: 10%; font-family: Arial, sans-serif;background-image: url(https://e1.pxfuel.com/desktop-wallpaper/288/797/desktop-wallpaper-red-chinese-dragon-chinese-red-dragon.jpg);}
    
    .container {
      height: 60%;
      width: 100%;  
      background-color: rgb(12, 12, 12);  
      background-size: cover;  
      background-position: center;   
    }

    .nav-bar {  
      display: flex;  
      align-items: center;  
      justify-content: space-between;  
      padding: 30px 80px;
    }

    .nav-bar .title {
      color: red;
      font-size: 50px;
    }

    .nav-bar p {
      position: absolute;
      margin-top: 120px;
      margin-left: 50px;
      color: #f0e5e5;
      font-size: 20px;
      font-weight: 500;
    }

    .menu li {
      list-style: none;
      display: inline-block;
    }

    .menu li a {
      text-decoration: none;
      color: #fff;
      font-size: 22px;
      font-weight: 600;
      margin-left: 25px;
      transition: .4s ease;
    }

    .menu li a:hover {
      color: rgb(253, 0, 13);
      padding: 10px 20px;
      border: 2px solid #fff;
    }

    .home {
      padding: 70px;
      text-align: center;
    }

    .title-1 {
      font-size: 56px;
      color: gold;
      font-weight: 600;
    }

    .home p {
      color: rgb(255, 255, 255);
      font-size: 25px;
      padding-top: 10px;
    }

    .image-row {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-top: 20px;
      flex-wrap: wrap;
    }

    .image-row img {
      width: 800px;
      height: 600px;
      object-fit: cover;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
      transition: transform 0.3s ease;
    }

    .image-row img:hover {
      transform: scale(1.05);
    }
  </style>
</head>  
<body>  
  <div class="container"> 
    <div class="nav-bar">  
      <h1 class="title">RED DRAGON CHINESE RESTAURANT</h1> 
      <p>Rich.Exquisite.Delightful.</p>  
      <ul class="menu"> 
        <li><a href="home.html">HOME</a></li>  
        <li><a href="menu.html">MENU</a></li> 
        <li><a href="admin.html">ADMIN</a></li>  
        <li><a href="contact.html">CONTACT</a></li> 
      </ul>  
    </div>
    <div class="home">
      <h1 class="title-1">"A taste of tradition in every bite — where the flavors of China come alive."</h1>
      <p>You're Invited to Feast at Red Dragon!

Join us for bold flavors, warm vibes, and a side of fortune.

From crispy spring rolls to sizzling stir-fries, Red Dragon Chinese Restaurant serves up the kind of delicious that makes chopsticks optional (but recommended).</p>
      
      <div class="image-row">
        <img src="image1.jpg" alt="Restaurant interior">
      </div>
    </div>
  </div>
</body>
</html>
```

## menu.html
```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;background-image: url(https://media-assets.swiggy.com/swiggy/image/upload/fl_lossy,f_auto,q_auto/xm7xnrxr6dht5bgzizqr);
            background-color: #080808;
            color: gold;
        }

        header {
            background-color: gold;
            color: #f40303;
            padding: 20px 0;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        nav ul {
            list-style-type: none;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        nav a {
            color: #f50505;
            text-decoration: none;
            font-size: 1.2rem;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #f4a261; /* Light orange on hover */
        }

        main {
            padding: 40px 20px;
            text-align: center;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #ffffff;
        }

        .menu-list {
            list-style-type: none;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            justify-items: center;
        }

        .menu-list li {
            width: 300px;
            background-color: #1d0404;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(225, 224, 224, 0.1);
            text-align: center;
        }

        .menu-list img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 15px;
        }

        .menu-list li p {
            font-size: 1.1rem;
            color: #fffdfd;
            font-weight: bold;
        }

        .menu-list li:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(255, 255, 255, 0.15);
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Our Menu</h1>
        <nav>
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="admin.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <h2>Food Items</h2>
        <ul class="menu-list">
            <li><img src="ramen noodles.jpg" alt="Food Item 1">Ramen Noodles- $30</li>
            <li><img src="spring roll.jpg" alt="Food Item 2">Spring Rools - $8</li>
            <li><img src="dumpling.jpg" alt="Food Item 3">Dumpling-$12</li>
            <li><img src="crab.jpg" alt="Food Item 4">Crab Rangoon - $7</li>
            <li><img src="sour.jpg" alt="Food Item 5">Sour Chicken - $15</li>
            <li><img src="kung.jpg" alt="Food Item 6">Kung Pao Park - $15</li>
            <li><img src="fish.jpg" alt="Food Item 7">Szechuan Fish - $26</li>
            <li><img src="mongolian.jpg" alt="Food Item 8">Mongolian Beef - $24</li>
            <li><img src="lo.jpg" alt="Food Item 9">Lo Mein Beef - $20</li>
            <li><img src="duck.jpg" alt="Food Item 10">Peking Duck - $30</li>
            <li><img src="tso.jpg" alt="Food Item 11">Tso Chicken - $26</li>
            <li><img src="tandoori.jpg" alt="Food Item 11">Tandoori - $16</li>
        </ul>
    </main>
    <footer>
        <p>&copy; Prethivirajan.L (212224040251)</p>
    </footer>
</body>
</html>

```

## admin.html
```html
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration</title>
    <style>
     *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

body {
    font-family: Arial, sans-serif;
    background-color: white;
    color: white;
}

header {
    background-color: gold;
    color: #ff0000;
    padding: 20px 0;
    text-align: center;
}

header h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
    gap: 20px;
}

nav a {
    color: #f80000;
    text-decoration: none;
    font-size: 1.2rem;
    transition: color 0.3s ease;
}

nav a:hover {
    color: #f4a261; 
}

main {
    padding: 40px 20px;
    text-align: center;
}

h2 {
    font-size: 2rem;
    margin-bottom: 20px;
    color: #333;
}


.team {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 30px;
    justify-items: center;
    margin-top: 30px;
}

.member {
    background-color: #090606;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.member img {
    width: 100%;
    height: auto;
    border-radius: 50%;
    margin-bottom: 15px;
    border: 4px solid #f4a261; 
}

.member h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
    color: #f2f2f2;
}

.member p {
    font-size: 1.1rem;
    color: #ffffff;
}

.member:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

h3 {
    margin-bottom: 10px;
    font-size: 1.5rem;
    color: #eae9e9;
}

footer {
    background-color: #333;
    color: #5b4f4f;
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
</style>
</head>
<body>
    <header>
        <h1>Administration Team</h1>
        <nav>
            <ul>
                <li><a href="home.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <h2>Meet Our Team</h2>
        <div class="team">
            <div class="member">
                <img src="ceo.jpg" alt="Member 1">
                <h3>Ajith</h3>
                <p>CEO</p>
            </div>
            <div class="member">
                <img src="dong.jpg" alt="Member 2">
                <h3>Dong Lee<h3>
                <p>Marketing Manager</p>
            </div>
            <div class="member">
                <img src="wick.jpg" alt="Member 3">
                <h3>Johnwick<h3>
                <p>Operations Manager</p>
            </div>
            <div class="member">
                <img src="prof.jpg" alt="Member 4">
                <h3>Sergio<h3>
                <p>HR Manager</p>
            </div>
            <div class="member">
                <img src="bale.jpg" alt="Member 5">
                <h3>Christian Bale<h3>
                <p>Executive Chef</p>
            </div>
            <div class="member">
                <img src="surraa.webp" alt="Member 6">
                <h3>Suraa<h3>
                <p>Customer Service Manger</p>
            </div>
        </div>
    </main>
</body>
</html>


```

## contact.html
```html
<<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact - RED DRAGON CHINESE RESTAURANT</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-image: url('https://images.unsplash.com/photo-1519181245277-cffeb31da2e3?fm=jpg&q=60&w=3000&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8Y2hpbmVzZSUyMGxhbnRlcm58ZW58MHx8MHx8fDA%3D');
      background-size: cover;
      background-position: center;
      color: #333;
    }

    #contact {
      background-color: lightcoral;
      padding: 80px 20px;
      margin: 400px auto;
      max-width: 800px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    #contact h2 {
      font-size: 5rem;
      margin-bottom: 30px;
      color: #333;
    }

    #contact p, address {
      font-size: 3rem;
      margin-bottom: 20px;
      color: #555;
    }

    address {
      font-style: normal;
    }
  </style>
</head>
<body>
  <section id="contact">
    <h2>Contact Us</h2>
    <p>Visit us at:</p>
    <address>
      143,jung-yang-lao,zhang matao,thailand<br>
      Phone: (+66) 81-456-9090<br>
      Email: sawadikathailand777@gmail.com
    </address>
  </section>
</body>
</html>

```


## OUTPUT:

![alt text](<WhatsApp Image 2025-10-31 at 09.32.53_4a8cdf97.jpg>)
![alt text](<WhatsApp Image 2025-10-31 at 09.33.18_79221de3.jpg>)
![alt text](<WhatsApp Image 2025-10-31 at 09.31.34_e836490f.jpg>)
![alt text](<WhatsApp Image 2025-10-31 at 09.31.39_ac90ed25.jpg>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
