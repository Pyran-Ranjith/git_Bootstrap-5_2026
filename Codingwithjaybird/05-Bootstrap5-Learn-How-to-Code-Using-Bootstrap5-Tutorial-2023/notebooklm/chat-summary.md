මෙම මූලාශ්‍රය මගින් **Bootstrap 5** භාවිතා කරමින් ඉතා කෙටි කාලයකින් **responsive** වෙබ් අඩවියක් නිර්මාණය කරන ආකාරය පිළිබඳව උපදෙස් ලබා දෙයි. මෙහිදී **CSS** හෝ **JavaScript** කේත ලිවීමෙන් තොරව, පූර්වයෙන් සකස් කරන ලද **navbars**, **carousels**, සහ **cards** වැනි උපාංග භාවිතා කරමින් වෘත්තීය මට්ටමේ වෙබ් පිටුවක් ගොඩනගන ආකාරය විස්තර කෙරේ. කැනඩාවේ සංචාරක කර්මාන්තය තේමාව කරගත් වෙබ් අඩවියක් උදාහරණයක් ලෙස යොදාගනිමින්, **Bootstrap Grid System** හරහා අන්තර්ගතය පෙළගස්වන ආකාරය මෙහි පෙන්වා දෙයි. මීට අමතරව, වෙබ් පිටුවකට පින්තූර එක් කිරීම, වර්ණ ගැන්වීම සහ විවිධ උපාංග සඳහා ගැලපෙන ලෙස පිටුව සකස් කරන ආකාරය පිළිබඳවද මෙහි මගපෙන්වීම් ඇතුළත් වේ. අවසාන වශයෙන්, වෙබ් අඩවියේ විවිධ කොටස් අතර ගමන් කිරීමට **navigation links** නිවැරදිව සම්බන්ධ කරන ආකාරය පිළිබඳව පැහැදිලි අවබෝධයක් මෙමගින් ලබා දෙයි. මෙම පාඩම මගින් නවක කේත කරන්නන්ට තමන්ගේම වෙබ් අඩවි නිර්මාණය කිරීමට අවශ්‍ය විශ්වාසය සහ ප්‍රායෝගික දැනුම ලබා දීම අරමුණු කරයි.

This response provides a comprehensive guide to building a responsive website with Bootstrap 5, based on the provided tutorial.

### Video Presentation Script

**00:00 - 02:00: Introduction and Setup**
*   **Key Concept:** Bootstrap 5 is a popular CSS framework for building **mobile-first, responsive websites** without writing custom CSS or JavaScript.
*   **Action:** Create a project folder with an `index.html` file and an images folder.
*   **Code Example:** Visit `getbootstrap.com` to copy the **Starter Template**, which includes the necessary CSS and JavaScript links.

**02:00 - 04:00: Navigation Bar**
*   **Key Concept:** Using pre-made components to speed up development.
*   **Action:** Copy a Navbar component from Bootstrap documentation. Replace text logos with an `<img>` tag.
*   **Code Example:**
    ```html
    <nav class="navbar ...">
      <img src="img/logo.jpg" alt="Logo" height="80">
      <!-- Links point to IDs for single-page scrolling -->
      <a class="nav-link" href="#destinations">Destinations</a>
    </nav>
    ```

**04:00 - 06:00: Image Carousel**
*   **Key Concept:** Modifying component structures.
*   **Action:** Add a fourth slide by duplicating an indicator button and a carousel item. Use **alt tags** for accessibility and `w-100` to ensure images fill the width.

**06:00 - 09:00: Main Container and Typography**
*   **Key Concept:** **Bootstrap Layout and Utility Classes**.
*   **Action:** Wrap content in a `<div class="container">`. Use utility classes for alignment and spacing.
*   **Code Example:**
    ```html
    <h1 class="text-center p-5 mb-5 mt-5">Tour Canada Today</h1>
    <div class="w-100 bg-dark-subtle p-3">...</div>
    ```

**09:00 - 12:00: The Grid System (Cards and Columns)**
*   **Key Concept:** **Responsive 12-column grid**.
*   **Action:** Create a row with three columns for cards. **Remove the fixed "18rem" width** from the default Bootstrap card code to make them fully responsive.
*   **Code Example:**
    ```html
    <div class="row">
      <div class="col"> <!-- Card 1 --> </div>
      <div class="col"> <!-- Card 2 --> </div>
      <div class="col"> <!-- Card 3 --> </div>
    </div>
    ```

**12:00 - 15:00: About & Contact Sections**
*   **Key Concept:** Using `col-6` for a 2x2 grid layout.
*   **Action:** Apply alternating background colors (e.g., `bg-secondary` and `bg-dark-subtle`) for visual interest.

**15:00 - End: Footer and Final Testing**
*   **Key Concept:** Global layout management.
*   **Action:** Place the footer **outside the main container** so it can span the full width of the browser. Test responsiveness by shrinking the browser.

---

### Slide Deck Outline for Beginners

*   **Slide 1: What is Bootstrap 5?**
    *   World's most popular CSS framework.
    *   Focus on **mobile-first** and **responsive** design.
    *   Build interactive sites without custom CSS/JS.
*   **Slide 2: Getting Started**
    *   The importance of the **Starter Template** (CSS/JS links).
    *   Basic folder structure: `index.html` and assets.
*   **Slide 3: Working with Components**
    *   Finding components on `getbootstrap.com` (Navbars, Carousels, Cards).
    *   Customizing components: Adding IDs and updating image sources.
*   **Slide 4: Layout & The Grid System**
    *   **The Container:** Centers content and provides padding.
    *   **Rows and Columns:** Dividing the page into 12 units (e.g., `col-6` for half-width).
*   **Slide 5: Bootstrap Utility Classes**
    *   **Spacing:** `p-5` (padding), `mb-5` (margin bottom).
    *   **Colors:** `bg-dark`, `text-white`, `bg-dark-subtle`.
    *   **Text:** `text-center`, `fs-1` (font size).
*   **Slide 6: Best Practices**
    *   Adding `alt` tags to images.
    *   Removing fixed widths (like `18rem`) for responsiveness.
    *   Closing div comments to stay organized.

---

### Important Code Snippets and Explanations

| Snippet | Explanation |
| :--- | :--- |
| `<div class="container">` | Centers your content and prevents it from hitting the browser edges. |
| `<div class="row">` | A wrapper for column divs that uses Flexbox for layout. |
| `class="w-100"` | A utility class that forces an element (like an image) to fill **100% of its container's width**. |
| `class="text-center"` | Easily centers text within any element. |
| `p-5`, `m-5` | Utility classes for **padding** and **margin**. The number (1-5) represents the degree of spacing. |
| `class="fs-1"` | Allows you to apply the **font size** of a Heading 1 to any text element, even if it's not an `<h1>` tag. |
| `href="#contact"` | Used in the Navbar to point to a specific section's **ID** (`id="contact"`) for single-page scrolling. |
| `text-decoration-none` | Removes the default underline from anchor (link) tags. |

මෙන්න වීඩියෝවේ අඩංගු තොරතුරු සහ උපදෙස් අනුව සකස් කරන ලද සම්පූර්ණ `index.html` ගොනුව. මෙහි Bootstrap 5 භාවිතා කර ඇති අතර, වීඩියෝවේ දැක්වෙන සියලුම උදාහරණ සහ responsive සැලසුම් ඇතුළත් වේ,.

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- Bootstrap 5 Starter Template එකෙන් ලබාගත් CSS link එක -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <title>Build a web page using bootstrap 5</title>
  </head>
  <body>

    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        <!-- Logo එක සහ උස 80 ලෙස සකස් කිරීම -->
        <a class="navbar-brand" href="#">
          <img src="IMG/logo.jpg" alt="Tour Canada Logo" height="80">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <!-- IDs මගින් single-page scrolling සක්‍රීය කිරීම, -->
            <li class="nav-item">
              <a class="nav-link" href="#destinations">Destinations</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#about">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Contact Us</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Carousel Section (ස්ලයිඩ 4ක් සහිතව), -->
    <div id="carouselExampleIndicators" class="carousel slide">
      <div class="carousel-indicators">
        <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
        <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
        <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
        <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3" aria-label="Slide 4"></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="IMG/lighthouse.jpg" class="d-block w-100" alt="Lighthouse">
        </div>
        <div class="carousel-item">
          <img src="IMG/geese.jpg" class="d-block w-100" alt="Geese">
        </div>
        <div class="carousel-item">
          <img src="IMG/mountains.jpg" class="d-block w-100" alt="Mountains">
        </div>
        <div class="carousel-item">
          <img src="IMG/falls.jpg" class="d-block w-100" alt="Falls">
        </div>
      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>

    <!-- Main Container ආරම්භය -->
    <div class="container">
      
      <!-- ප්‍රධාන ශීර්ෂය සහ පෙළ, -->
      <h1 class="text-center p-5 mb-5 mt-5">Tour Canada Today</h1>
      
      <div class="w-100 bg-dark-subtle p-3 mb-5 mt-5">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. (Lorem 100 placeholders here...)</p>
        <!-- Bootstrap Button -->
        <button type="button" class="btn btn-primary btn-lg">Book your trip now</button>
      </div>

      <!-- Destinations Section (Grid System භාවිතා කර), -->
      <h2 id="destinations" class="fs-1 text-center p-5 mb-5 mt-5">Popular Destinations</h2>
      
      <div class="row">
        <!-- Card 1 - Banff (Responsive බව සඳහා fixed width ඉවත් කර ඇත), -->
        <div class="col">
          <div class="card">
            <img src="IMG/mountains.jpg" class="card-img-top" alt="Mountains">
            <div class="card-body">
              <h5 class="card-title">Banff</h5>
              <p class="card-text">Lorem ipsum dolor sit amet... (Lorem 30)</p>
              <a href="#" class="btn btn-primary">Read more</a>
            </div>
          </div>
        </div>
        <!-- Card 2 - Peggy's Cove -->
        <div class="col">
          <div class="card">
            <img src="IMG/lighthouse.jpg" class="card-img-top" alt="Lighthouse">
            <div class="card-body">
              <h5 class="card-title">Peggy's Cove</h5>
              <p class="card-text">Lorem ipsum dolor sit amet... (Lorem 30)</p>
              <a href="#" class="btn btn-primary">Read more</a>
            </div>
          </div>
        </div>
        <!-- Card 3 - Yukon -->
        <div class="col">
          <div class="card">
            <img src="IMG/yukon.jpg" class="card-img-top" alt="Yukon">
            <div class="card-body">
              <h5 class="card-title">Yukon</h5>
              <p class="card-text">Lorem ipsum dolor sit amet... (Lorem 30)</p>
              <a href="#" class="btn btn-primary">Read more</a>
            </div>
          </div>
        </div>
      </div>

      <!-- About Us Section (col-6 භාවිතා කර Grid 4ක්), -->
      <h2 id="about" class="fs-1 text-center p-5 mb-5 mt-5">About</h2>
      
      <div class="row text-center">
        <!-- Block 1: Rates -->
        <div class="col-6">
          <div class="bg-secondary text-white p-5 m-2">
            <h2>Rates</h2>
            <p>Lorem ipsum dolor sit amet... (Lorem 50)</p>
          </div>
        </div>
        <!-- Block 2: Fees -->
        <div class="col-6">
          <div class="bg-dark-subtle p-5 m-2">
            <h2>Fees</h2>
            <p>Lorem ipsum dolor sit amet... (Lorem 50)</p>
          </div>
        </div>
        <!-- Block 3: Popular Sites -->
        <div class="col-6">
          <div class="bg-dark-subtle p-5 m-2">
            <h2>Popular Sites</h2>
            <p>Lorem ipsum dolor sit amet... (Lorem 50)</p>
          </div>
        </div>
        <!-- Block 4: Features -->
        <div class="col-6">
          <div class="bg-secondary text-white p-5 m-2">
            <h2>Features</h2>
            <p>Lorem ipsum dolor sit amet... (Lorem 50)</p>
          </div>
        </div>
      </div>

      <!-- Contact Us Section -->
      <h2 id="contact" class="fs-1 text-center p-5 mb-5 mt-5">Contact Us</h2>
      <div class="w-100 bg-dark-subtle p-3 mb-5 mt-5 text-center">
        <p>
          <a href="mailto:abc@def.com" class="text-white text-decoration-none">Contact us for more information</a>
        </p>
      </div>

      <!-- Transition Image -->
      <h2 class="fs-1 text-center p-5 mb-5 mt-5">Relax in beautiful Canada</h2>
      <img src="IMG/vacation.jpg" class="w-100 mb-5" alt="Vacation">

    </div> <!-- Main Container අවසානය -->

    <!-- Footer (Container එකෙන් පිටත, සම්පූර්ණ පළල සඳහා), -->
    <footer class="bg-dark text-white text-center p-5 mt-5">
      <p>&copy; Tour Canada Today</p>
      <a href="mailto:abc@def.com" class="text-white">Email us</a>
    </footer>

    <!-- Bootstrap 5 JavaScript -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
  </body>
</html>
```

### වැදගත් කරුණු:
*   **Responsive බව:** වීඩියෝවේ දැක්වෙන පරිදි Cards වල ඇති `width: 18rem` කොටස ඉවත් කර ඇති අතර, `col` සහ `col-6` වැනි grid classes භාවිතා කර ඇත,.
*   **Navigation:** Nav links හරහා අදාළ ID ඇති ස්ථානයට (උදා: `#destinations`) ස්ක්‍රෝල් කිරීමට හැකි වන සේ සකසා ඇත,.
*   **පින්තූර:** `IMG/` ෆෝල්ඩරය තුළ `logo.jpg`, `lighthouse.jpg`, `geese.jpg`, `mountains.jpg`, `falls.jpg`, `yukon.jpg` සහ `vacation.jpg` නමින් පින්තූර තිබිය යුතු බව උපකල්පනය කර ඇත,,.

මෙම වීඩියෝ මාලාවේ නිර්මාණකරු පවසන පරිදි, මෝඩල් (Modal) යනු බූට්ස්ට්‍රැප් හි ඇති 'pre-made components' වලින් එකකි. මෙම වීඩියෝවේ ඇති උපදෙස් අනුව ඔබේ වෙබ් පිටුවට මෝඩල් එකක් එකතු කර ගැනීමට පහත පියවර අනුගමනය කළ හැකිය:

1.  **getbootstrap.com වෙබ් අඩවියට පිවිසෙන්න:** වීඩියෝවේ සඳහන් පරිදි සියලුම බූට්ස්ට්‍රැප් උපාංග ලබා ගැනීමට මෙම වෙබ් අඩවිය භාවිතා කළ යුතුය.
2.  **Components අංශය වෙත යන්න:** වෙබ් අඩවියේ "Docs" යටතේ ඇති **Components** අංශය වෙත යන්න.
3.  **Modal තෝරාගන්න:** එහි ඇති ලැයිස්තුවෙන් **Modal** යන්න තෝරා ඔබට අවශ්‍ය මෝඩල් මාදිලියේ කේතය (markup) කොපි කරගන්න.
4.  **HTML ගොනුවට ඇතුළත් කරන්න:** කොපි කරගත් කේතය ඔබේ `index.html` ගොනුව තුළට පේස්ට් කරන්න.
5.  **ක්‍රියාත්මක කරන ආකාරය:** සාමාන්‍යයෙන් මෝඩල් එකක් විවෘත කිරීමට බූට්ස්ට්‍රැප් බටන් (button) එකක් අවශ්‍ය වේ.

මෙම වීඩියෝවේ මෝඩල් සඳහා වන නිශ්චිත කේතය පෙන්වා නොමැති අතර, එහි නිර්මාණකරු පවසන්නේ ඉදිරි වීඩියෝවකදී මෝඩල් සහ ඇකෝඩියන් (accordions) වැනි දෑ භාවිතා කරන ආකාරය උගන්වන බවයි. එබැවින් ඔබට අවශ්‍ය විශේෂිත කේත ලබා ගැනීමට බූට්ස්ට්‍රැප් නිල වෙබ් අඩවියේ ඇති ලේඛන (documentation) භාවිතා කරන ලෙස ඔහු උපදෙස් දෙයි.

