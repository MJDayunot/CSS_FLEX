# CSS_FLEX

## What is Flexbox?
CSS Flexbox, or the Flexible Box Layout, is a layout model designed to help arrange items within a container, even when their sizes are unknown or dynamic. Flexbox allows easy alignment, distribution, and responsive adjustments of elements, making it ideal for creating adaptive and efficient layouts for various screen sizes.

## Key Flexbox Properties

| Property         | Description                                                                                      |
|------------------|--------------------------------------------------------------------------------------------------|
| `display: flex`  | Enables Flexbox for the container, making it a flex container.                                   |
| `flex-wrap`      | Controls item wrapping within the container (`nowrap`, `wrap`, `wrap-reverse`).                 |
| `justify-content`| Aligns items along the main axis (horizontal alignment). Common values: `center`, `space-between`.|
| `align-items`    | Aligns items along the cross axis (vertical alignment). Common values: `center`, `flex-start`.   |
| `gap`            | Defines consistent spacing between flex items.                                                   |

## HTML Code 

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Product Layout</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
<h1>Product Layout</h1>
<div class="product-container">
  <div class="product-item">Laptop</div>
  <div class="product-item">Smartphone</div>
  <div class="product-item">Headphones</div>
  <div class="product-item">Smartwatch</div>
  <div class="product-item">Camera</div>
</div>
</body>
</html>



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Employee Cards</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
<h1>Employee Cards</h1>
<div class="employee-container">
    <div class="employee-card">
        <h3>Daniel Dionisio</h3>
        <p>Position: Manager</p>
    </div>
    <div class="employee-card">
        <h3>Mary Grace Dayunot</h3>
        <p>Position: Developer</p>
    </div>
    <div class="employee-card">
        <h3>Aerrol Glen Agojo</h3>
        <p>Position: Designer</p>
    </div>
</div>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Student Profiles</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
<h1>Student Profiles</h1>
<div class="student-container">
  <div class="student-profile">
    <h3>John Reyes</h3>
    <p>Grade: 10</p>
  </div>
  <div class="student-profile">
    <h3>Maria Santos</h3>
    <p>Grade: 11</p>
  </div>
  <div class="student-profile">


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog Posts</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
<h1>Latest Blog Posts</h1>
<div class="blog-container">
    <div class="blog-post">
        <h3>The Future of Web Development</h3>
        <p>Web development is evolving rapidly with new technologies and frameworks. In this post, we explore the trends that will shape the future, including Web3, AI integration, and the growing importance of performance optimization.</p>
    </div>
    <div class="blog-post">
        <h3>How to Master CSS Flexbox</h3>
        <p>Flexbox is a powerful tool for creating responsive layouts. In this tutorial, we cover everything from basic concepts to advanced use cases, ensuring you have a solid understanding of how to use Flexbox in your projects.</p>
    </div>
    <div class="blog-post">
        <h3>Understanding JavaScript Promises</h3>
        <p>Promises are an essential part of modern JavaScript, allowing asynchronous code to be handled more effectively. This article breaks down promises, explaining how they work and how to use them to avoid callback hell.</p>
    </div>
</div>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recipe Cards</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
<h1>Recipe Cards</h1>
<div class="recipe-container">
    <div class="recipe-card">
        <h3>Classic Pancakes</h3>
        <p>Ingredients: Flour, Sugar, Eggs</p>
        <p>Instructions: Mix all ingredients and bake on a griddle.</p>
    </div>
    <div class="recipe-card">
        <h3>Grilled Chicken</h3>
        <p>Ingredients: Chicken, Spices, Olive Oil</p>
        <p>Instructions: Marinate chicken with spices and grill.</p>
    </div>
    <div class="recipe-card">
        <h3>Cheesy Pasta</h3>
        <p>Ingredients: Pasta, Tomato Sauce, Cheese</p>
        <p>Instructions: Cook pasta, add tomato sauce, and sprinkle with cheese.</p>
    </div>
</div>
</body>
</html>

    <h3>Kevin Dela Cruz</h3>
    <p>Grade: 12</p>
  </div>
</div>
</body>
</html>


CSS STYLES

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f9f9f9;
}

h1 {
    text-align: center;
    color: #333;
    margin-top: 20px;
}

.product-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    padding: 20px;
    background-color: #f0f4c3;
}

.product-item {
    background-color: #fff9c4;
    padding: 20px;
    border: 1px solid #ddd;
    width: 150px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.product-item:hover {
    transform: scale(1.05);
}

.employee-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 20px;
    background-color: #e3f2fd;
}

.employee-card {
    background-color: #bbdefb;
    border-radius: 8px;
    padding: 15px;
    width: 200px;
    text-align: center;
    margin: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.employee-card:hover {
    transform: scale(1.05);
}

.student-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 20px;
    background-color: #ede7f6;
}

.student-profile {
    background-color: #d1c4e9;
    border-radius: 8px;
    padding: 15px;
    width: 180px;
    text-align: center;
    margin: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.student-profile:hover {
    transform: scale(1.05);
}

.blog-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 20px;
    background-color: #fff3e0;
}

.blog-post {
    background-color: #ffe0b2;
    border-radius: 8px;
    padding: 15px;
    width: 250px;
    text-align: center;
    margin: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.blog-post:hover {
    transform: scale(1.05);
}

.recipe-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 20px;
    background-color: #fce4ec;
}

.recipe-card {
    background-color: #f8bbd0;
    border-radius: 8px;
    padding: 15px;
    width: 220px;
    text-align: center;
    margin: 10px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.recipe-card:hover {
    transform: scale(1.05);
}

.product-item,
.employee-card,
.student-profile,
.blog-post,
.recipe-card {
    background-color: #ffffff;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 15px;
    margin: 10px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}


