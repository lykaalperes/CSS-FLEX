# CSS_FLEX

## What is Flexbox?
CSS Flexbox, or Flexible Box Layout, is a CSS module designed to streamline the arrangement of elements within a container. It ensures that items are well-aligned, distributed, and adaptable, even when their sizes vary. Flexbox is highly effective for creating responsive layouts that adjust seamlessly to different screen sizes.

## Key Flexbox Properties

| Property         | Description                                                                                      |
|------------------|--------------------------------------------------------------------------------------------------|
| `display: flex`  | Activates Flexbox on a container, making it a "flex container."                                 |
| `flex-wrap`      | Manages whether items wrap onto multiple lines (nowrap, wrap, wrap-reverse).                |
| `justify-content`| Distributes items along the main axis (horizontal alignment). Popular options: center, space-around.|
| `align-items`    | Aligns items on the cross axis (vertical alignment). Values include center, flex-end.   |
| `gap`            | Specifies uniform spacing between flex items for cleaner layouts.                              |

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
        <h3>Lyka Alperes</h3>
        <p>Position: UX UI Designer</p>
    </div>
    <div class="employee-card">
        <h3>Mary Jane Dayunot</h3>
        <p>Position: Lead Programmer</p>
    </div>
    <div class="employee-card">
        <h3>Mark Laureano</h3>
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



## CSS STYLES
CSS


body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f6f8;
}

h1 {
    text-align: center;
    color: #2d3436;
    margin: 20px 0;
}

.product-container, .employee-container, .student-container, .blog-container, .recipe-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 16px;
    padding: 20px;
}

.product-item, .employee-card, .student-profile, .blog-post, .recipe-card {
    background-color: #ffffff;
    border: 1px solid #e0e0e0;
    border-radius: 10px;
    padding: 20px;
    width: 180px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s, box-shadow 0.2s;
}

.product-item:hover, 
.employee-card:hover, 
.student-profile:hover, 
.blog-post:hover, 
.recipe-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 8px rgba(0, 0, 0, 0.2);
}

/* Section-specific colors for better contrast */
.product-container {
    background-color: #eafbea;
}

.employee-container {
    background-color: #e8f5fe;
}

.student-container {
    background-color: #f3e5f5;
}

.blog-container {
    background-color: #fff8e1;
}

.recipe-container {
    background-color: #ffebee;
}

/* Responsive styles */
@media (max-width: 600px) {
    .product-item, .employee-card, .student-profile, .blog-post, .recipe-card {
        width: 100%;
    }
}
