---
layout: minima
title: About
permalink: /about/
comments: true
---

## As a conversation Starter
Some Videogames I play:
-Roblox
-Fortnite

Some Animes I Watch:
-One piece
-Solo Leveling
-Dragon Ball
-Jujutsu Kaisen

My Two Favorite Quotes:
"I can accept failure, everyone fails at something. But I can't accept not trying"- Micheal Jordan and "If you do the work, you get rewarded. There are no shortcuts in life."- Micheal Jordan

## Here are some places I have lived.

<comment>
Flags are made using Wikipedia images
</comment>

<style>
    /* Style looks pretty compact, 
       - grid-container and grid-item are referenced the code 
    */
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
        gap: 10px;
    }
    .grid-item {
        text-align: center;
    }
    .grid-item img {
        width: 100%;
        height: 100px; /* Fixed height for uniformity */
        object-fit: contain; /* Ensure the image fits within the fixed height */
    }
    .grid-item p {
        margin: 5px 0; /* Add some margin for spacing */
    }

    /* Food image styling for the favorite foods grid */
    .food-img {
        width: 100%;
        height: 100px;
        object-fit: cover;
        border-radius: 4px;
        display: block;
        margin-bottom: 8px;
    }

    .image-gallery {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 10px;
        }

    .image-gallery img {
        max-height: 150px;
        object-fit: cover;
        border-radius: 5px;
    }
</style>

<!-- This grid_container class is used by CSS styling and the id is used by JavaScript connection -->
<div class="grid-container" id="grid_container">
    <!-- content will be added here by JavaScript -->
</div>

<script>
    // 1. Make a connection to the HTML container defined in the HTML div
    var container = document.getElementById("grid_container"); // This container connects to the HTML div

    // 2. Define a JavaScript object for our http source and our data rows for the Living in the World grid
    var http_source = "https://upload.wikimedia.org/wikipedia/commons/";
    var living_in_the_world = [
        {"flag": "0/01/Flag_of_California.svg", "greeting": "Hey", "description": "California - forever"},
    ];

    // 3a. Consider how to update style count for size of container
    // The grid-template-columns has been defined as dynamic with auto-fill and minmax

    // 3b. Build grid items inside of our container for each row of data
    for (const location of living_in_the_world) {
        // Create a "div" with "class grid-item" for each row
        var gridItem = document.createElement("div");
        gridItem.className = "grid-item";  // This class name connects the gridItem to the CSS style elements
        // Add "img" HTML tag for the flag
        var img = document.createElement("img");
        img.src = http_source + location.flag; // concatenate the source and flag
        img.alt = location.flag + " Flag"; // add alt text for accessibility

        // Add "p" HTML tag for the description
        var description = document.createElement("p");
        description.textContent = location.description; // extract the description

        // Add "p" HTML tag for the greeting
        var greeting = document.createElement("p");
        greeting.textContent = location.greeting;  // extract the greeting

        // Append img and p HTML tags to the grid item DIV
        gridItem.appendChild(img);
        gridItem.appendChild(description);
        gridItem.appendChild(greeting);

        // Append the grid item DIV to the container DIV
        container.appendChild(gridItem);
    }
</script>

## Here are my favorite foods

<h2>Favorite TV Shows</h2>
<div class="grid-container" id="shows_grid">
    <!-- Favorite shows will be added here by JavaScript -->
</div>


<script>
    var favorite_shows = [
        {
            "img": "https://github.com/user-attachments/assets/e714f34b-77fc-42e3-9a32-3b8a0072d988",
            "title": "One Piece"
        },
        {
            "img": "https://github.com/user-attachments/assets/9aa11b4a-6f8d-42c2-8f96-dd857dabf952",
            "title": "Solo Leveling"
        },
        {
            "img": "https://github.com/user-attachments/assets/382dd0c1-291e-48a8-9cb5-b61886573c47",
            "title": "Jujutsu Kaisen"
        }
    ];


    var showsContainer = document.getElementById("shows_grid");
    for (const show of favorite_shows) {
        var item = document.createElement("div");
        item.className = "grid-item";
        var img = document.createElement("img");
        img.src = show.img;
        img.alt = show.title;
        var p = document.createElement("p");
        p.textContent = show.title;
        item.appendChild(img);
        item.appendChild(p);
        showsContainer.appendChild(item);
    }
</script>






<!-- Favorite Food grid -->
<h2>Favorite Food</h2>
<div class="grid-container" id="food_grid">
    <!-- Favorite food will be added here by JavaScript -->
</div>


<script>
    var favorite_food = [
        {
            "img": "https://github.com/user-attachments/assets/25c5c0fa-0be3-4212-9897-12b345851a13",
            "title": "Pizza"
        },
        {
            "img": "https://github.com/user-attachments/assets/4320b238-2926-4a3c-9c34-622fb47669bc",
            "title": "Sushi"
        },
        {
            "img": "https://github.com/user-attachments/assets/0c1a33e0-04b1-43b8-9ee4-39946316da81",
            "title": "Burgers"
        },
        {
            "img": "https://github.com/user-attachments/assets/a81d8c62-9fda-40c9-8f38-46aed9bcbbe0",
            "title": "Ramen"
        }
    ];


    var gamesContainer = document.getElementById("food_grid");
    for (const game of favorite_food) {
        var item = document.createElement("div");
        item.className = "grid-item";
        var img = document.createElement("img");
        img.src = food.img;
        img.alt = food.title;
        var p = document.createElement("p");
        p.textContent = game.title;
        item.appendChild(img);
        item.appendChild(p);
        gamesContainer.appendChild(item);
    }
</script>

### Journey through Life

Here is what I did at those places

-I was born here in California in 2010 and stayed here my whole life
-🏫 I went to Hiltop Elementary school in 2015 since they had a preschool there and stayed until 2022
-🏫 I moved over here to 4s Ranch and went to Oak Valley Middle School in 2022, graduated in 2024
-👨‍🏫 I then came to Del Norte High School in 2024 and ever since then the story continues until I graduate in 2028

### Culture, Family, and Fun

I am super close with my family especially my mom.
My family has definitely a big inspiration in my life and encourages me to better myself everyday.
I love spending time with my family and go on vacations with them.

<comment>
Gallery of Pics:
</comment>
<div class="image-gallery">
<img src="aydend456/student/images/tokyo-tower.jpg" alt="Image 1">
<img src="aydend456/student/images/my-mom-and-I.jpg" alt="Image 2">
<img src="aydend456/student/images/ayden.jpg" alt="Image 3">
</div>