මෙම මූලාශ්‍රය මගින් **Bootstrap 5** භාවිතා කරමින් ඉතා වේගයෙන් සහ පහසුවෙන් **ප්‍රතිචාරාත්මක වෙබ් අඩවි** නිර්මාණය කරන ආකාරය පැහැදිලි කරයි. මෙහිදී වෙබ් සංවර්ධකයින් අතර වඩාත් ජනප්‍රිය අංග වන **Navbars**, **Carousels**, සහ **Accordions** වැනි මෙවලම් පහසුවෙන් වෙබ් පිටුවකට එක් කරන ආකාරය පෙන්වා දෙයි. මීට අමතරව, තොරතුරු ප්‍රදර්ශනය කිරීමට උපකාරී වන **Modals** සහ දත්ත සංවිධානය කිරීමට භාවිතා කරන **Cards** වැනි අංගයන්ගේ ඇති වැදගත්කම මෙහි අවධාරණය කෙරේ. සූදානම් කළ කේත කොටස් පිටපත් කර අවශ්‍ය පරිදි වෙනස් කිරීමෙන් **ආකර්ෂණීය නිමාවක්** සහිත වෙබ් අඩවියක් ගොඩනගන ආකාරය මෙහි සවිස්තරාත්මකව දක්වා ඇත. අවසාන වශයෙන්, නවක සංවර්ධකයින්ට තම **කේතකරණ හැකියාවන්** වර්ධනය කර ගැනීමට අවශ්‍ය වටිනා උපදෙස් රැසක් මෙමගින් ඉදිරිපත් කරයි.

Based on the source provided, the following is a structural representation of the HTML and components discussed in the video. The video emphasizes using the **Bootstrap 5 starter template** and copying code snippets directly from the official Bootstrap documentation to build responsive websites.

### **1. HTML Structure (Starter Template & Layout)**
The video starts with a basic Bootstrap 5 template and organizes content within a responsive grid system.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Bootstrap 5 CSS would be linked here as part of the starter template -->
</head>
<body>
    <!-- Navbar Component -->
    <!-- Content is placed inside a container for proper width -->
    <div class="container">
        
        <!-- Carousel Component -->

        <!-- Accordion Component -->

        <!-- Modal Trigger Button -->

        <!-- Grid System for Cards -->
        <div class="row">
            <div class="col-4">
                <!-- Vertical Card (Kitchen Sink) -->
            </div>
            <div class="col-8">
                <!-- Horizontal Card -->
            </div>
        </div>
    </div>

    <!-- Modal Component -->

    <!-- Bootstrap 5 JS Bundle would be linked here -->
</body>
</html>
```

---

### **2. The 5 Popular Components**

#### **I. Navbar**
*   **Features:** Includes a mix of regular links and dropdown links.
*   **Styling:** Can be changed to a dark theme by applying the classes `navbar-dark` and `bg-dark`.
*   **Responsiveness:** Automatically collapses into a **hamburger menu** on smaller screens.

#### **II. Carousel**
*   **Features:** The video highlights a version with **indicators**, descriptions, and details for each slide.
*   **Customization:** Images from external sites like Pixabay are added manually to the `<img>` tags within the carousel code.

#### **III. Accordion**
*   **Features:** Uses a "stay open" variety where items can remain expanded.
*   **Content:** The items are renamed to **"item one"**, **"item two"**, and **"item three"**.
*   **Interaction:** Users click arrows to open and close details for each item.

#### **IV. Modal**
*   **Type:** The **static backdrop modal** is selected, which requires a button to trigger it.
*   **Content:** The source demonstrates adding a paragraph tag with approximately 100 words of placeholder text (`lorem 100`) to the modal body.

#### **V. Cards (The Author's Favorite)**
*   **Vertical "Kitchen Sink" Card:** Includes images, titles, text, and buttons. 
*   **Horizontal Card:** Placed within a specific column (`col-8`) to demonstrate a different orientation.
*   **Grid Integration:** Cards are placed within a **12-column grid system** using `row` and `col` classes to ensure they are responsive and correctly sized (e.g., removing preset widths like `18rem` to let the grid control them).

### **3. CSS and JavaScript**
*   **CSS:** No custom CSS is written in the video; instead, the author relies on **Bootstrap's built-in classes** (like `container`, `row`, `navbar-dark`, and `bg-dark`) for styling and layout.
*   **JavaScript:** The functionality for the hamburger menu, carousel transitions, accordion toggles, and modal pop-ups is handled automatically by the **Bootstrap 5 JavaScript bundle** included in the starter template.

