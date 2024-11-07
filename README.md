# Activity 26 CSS FLEX

# Instruction:
* Apply CSS Flexbox on 5 pages (e.g., product layout, employee cards, student profiles, etc.)

* Name your repository CSS_FLEX

* Add documentation in the README.md file of your repository

* Submit the GitHub repository link

* Deadline: December 5, 2024

## Pages and Layouts
1. **Product Layout**: Displays products in a responsive grid.
2. **Employee Cards**: Shows employee profiles in a card format.
3. **Student Profiles**: Lists student profiles with images.
4. **Gallery**: A flexible, responsive image gallery.
5. **Services**: Highlights different services.

## How to Use Flexbox
- `display: flex;` - Defines a flex container.
- `flex-wrap: wrap;` - Allows items to wrap onto new rows.
- `justify-content` - Aligns items horizontally within the container.


index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ACT 26 Responsive Flexbox Layout</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
    
  <!-- Product Layout Section -->
  <section class="section">
    <h2>Product Layout</h2>
    <div class="container">
      <div class="card">
        <img src="6154651727186477732.jpg" alt="Product 1">
        <h3>Product 1</h3>
        <p>Labubu 1</p>
        <button>Buy Now</button>
      </div>
      <div class="card">
        <img src="6154651727186477732.jpg" alt="Product 2">
        <h3>Product 2</h3>
        <p>Labubu 2</p>
        <button>Buy Now</button>
      </div>
      <div class="card">
        <img src="6154651727186477732.jpg" alt="Product 3">
        <h3>Product 3</h3>
        <p>Labubu 3</p>
        <button>Buy Now</button>
      </div>
    </div>
  </section>

  <!-- Employee Cards Section -->
  <section class="section">
    <h2>Employee Cards</h2>
    <div class="container">
      <div class="card">
        <img src="em1.jpg" alt="Employee 1">
        <h3>Mary</h3>
        <p>Position: Developer</p>
      </div>
      <div class="card">
        <img src="em2.jpg" alt="Employee 2">
        <h3>Joy</h3>
        <p>Position: Designer</p>
      </div>
      <div class="card">
        <img src="em3.jpg" alt="Employee 3">
        <h3>John</h3>
        <p>Position: Manager</p>
      </div>
    </div>
  </section>

  <!-- Student Profiles Section -->
  <section class="section">
    <h2>Student Profiles</h2>
    <div class="container">
      <div class="card">
        <img src="image.png" alt="Student 1">
        <h3>John</h3>
        <p>Course: Computer Science</p>
      </div>
      <div class="card">
        <img src="image.png" alt="Student 2">
        <h3>Johnson</h3>
        <p>Course: Information Technology</p>
      </div>
      <div class="card">
        <img src="image.png" alt="Student 3">
        <h3>Ken</h3>
        <p>Course: Business</p>
      </div>
    </div>
  </section>

  <!-- Gallery Section -->
  <section class="section">
    <h2>Gallery</h2>
    <div class="container">
      <div class="card">
        <img src="flo1.jpg" alt="">
      </div>
      <div class="card">
        <img src="flo2.jpg" alt="">
      </div>
      <div class="card">
        <img src="flo3.jpg" alt="">
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section class="section">
    <h2>Our Services</h2>
    <div class="container">
      <div class="card">
        <h3>Service 1</h3>
        <img src="serves.jpeg" alt="Gallery Image 2">
      </div>
      <div class="card">
        <h3>Service 2</h3>
        <img src="serves.jpeg" alt="Gallery Image 2">
      </div>
      <div class="card">
        <h3>Service 3</h3>
        <img src="serves.jpeg" alt="Gallery Image 2">
      </div>
    </div>
  </section>
</body>
</html>
```
styles.css

```
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  
  body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    padding: 20px;
    background-color: #f9f9f9;
  }
  
  h2 {
    margin-bottom: 20px;
    font-size: 1.8em;
    text-align: left;
    color: #333;
  }
  
  .section {
    margin-bottom: 40px;
  }
  
  .container {
    display: grid;              
    gap: 16px;                  
    grid-template-columns: 1fr; 
  }
  
  .card {
    background-color: #fff;
    padding: 16px;
    border: 1px solid #ddd;
    border-radius: 8px;
    text-align: center;
  }
  
  .card img {
    width: 100%;
    height: auto;
    border-radius: 8px;
  }
  
  .card h3 {
    font-size: 1.2em;
    margin-top: 8px;
  }
  
  .card p {
    font-size: 0.9em;
    margin: 8px 0;
  }
  
  .card button {
    padding: 8px 16px;
    margin-top: 8px;
    background-color: #0bc55f;
    color: #fff;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  
  .card button:hover {
    background-color: #ed0909;
  }
  
  /* Responsive adjustments (optional, as grid-template-columns handles responsiveness well) */
  @media (min-width: 600px) {
    .container {
        grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); /* More space for larger screens */
    }
  }
  
  
```

## OutPut
![Screenshot_7-11-2024_12326_](https://github.com/user-attachments/assets/4de1c4a8-de37-4e5a-bba1-f012cf1c914a)
