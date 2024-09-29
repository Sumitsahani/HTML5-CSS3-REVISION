
### **1. CSS3 (Cascading Style Sheets 3)**

**CSS3** ka matlab hai Cascading Style Sheets ka teesra version. Yeh web pages ko style karne ke liye use hota hai. CSS3 ne bahut saare naye features introduce kiye hain jo styling ko aur bhi powerful banate hain, jaise:

- **Flexbox**: Iska use elements ko horizontal ya vertical align karne ke liye hota hai, jisse responsive layouts create kiye ja sakte hain.
  
- **Grid Layout**: Yeh complex layouts ko manage karne mein help karta hai, jahan aap rows aur columns ka istemal karte hain.

- **Animations aur Transitions**: Inke through aap elements ko smoothly animate kar sakte hain, jaise kisi button ka hover effect ya kisi div ka slide-in effect.

- **Media Queries**: Yeh website ko responsive banane ke liye use hote hain, jisse different devices par layout aur styling change hoti hai.

#### **Definition**:
CSS3 ek advanced styling language hai jo web pages ko design karne mein madad karta hai. Isme naye features jaise **Flexbox, Grid, Animations, aur Media Queries** shamil hain, jo website ko zyada interactive aur responsive banate hain.

---

### **2. Box Model**

**Box Model** CSS ka ek fundamental concept hai. Har HTML element ko ek box ke roop mein treat kiya jata hai, jo chaar main parts mein divided hota hai:

- **Content**: Yeh element ka actual content hota hai, jaise text ya images.
  
- **Padding**: Yeh content ke aas-paas ka space hota hai. Padding se content aur border ke beech mein distance milta hai.

- **Border**: Yeh element ke outer edge par hota hai. Border ka thickness aur style customize kiya ja sakta hai.

- **Margin**: Yeh box ke bahar ka space hota hai, jo doosre elements se distance create karta hai.

**Box Model** ka samajhna zaroori hai kyunki yeh elements ke size aur layout ko control karta hai.

#### **Definition**:
Box Model ek concept hai jisme har HTML element ko ek box ki tarah dekha jata hai. Isme chaar parts hote hain: **Content, Padding, Border, aur Margin**, jo element ki positioning aur spacing ko define karte hain.

---

### **3. Different Ways to Include CSS in a Web Page**

CSS ko web page mein include karne ke teen tarike hain:

1. **Inline CSS**: Yeh directly HTML element ke andar style attribute ke through use hota hai. Yeh quick styling ke liye acha hota hai lekin maintenance mein mushkil hota hai.
   ```html
   <h1 style="color: red;">Hello World!</h1>
   ```

2. **Internal CSS**: Yeh `<style>` tag ke andar HTML document ke `<head>` section mein likha jata hai. Iska use tab hota hai jab aapko ek hi page par styles apply karne hain.
   ```html
   <head>
       <style>
           h1 { color: blue; }
       </style>
   </head>
   ```

3. **External CSS**: Yeh ek separate `.css` file hoti hai jo HTML document ke `<head>` section mein link kiya jata hai. Yeh best practice hai kyunki yeh code ko modular aur maintainable banata hai.
   ```html
   <head>
       <link rel="stylesheet" href="styles.css">
   </head>
   ```

#### **Definition**:
CSS ko web page mein include karne ke teen tarike hain: **Inline CSS**, jo element ke andar likha jata hai; **Internal CSS**, jo `<style>` tag ke andar hota hai; aur **External CSS**, jo alag CSS file se link hota hai. External CSS best practice hai kyunki isse code maintain karna aasaan hota hai.

---

### **4. All Selectors in CSS**

CSS selectors woh patterns hain jo elements ko select karne ke liye use hote hain. Kuch common selectors hain:

- **Universal Selector (`*`)**: Yeh sabhi elements ko target karta hai.
  ```css
  * { margin: 0; padding: 0; }
  ```

- **Type Selector**: Yeh specific HTML elements ko target karta hai.
  ```css
  p { color: green; }
  ```

- **Class Selector (`.`)**: Yeh specific class ke elements ko target karta hai.
  ```css
  .myClass { font-size: 20px; }
  ```

- **ID Selector (`#`)**: Yeh specific ID wale element ko target karta hai.
  ```css
  #myId { background-color: yellow; }
  ```

- **Attribute Selector**: Yeh specific attributes wale elements ko target karta hai.
  ```css
  input[type="text"] { border: 1px solid black; }
  ```

- **Descendant Selector**: Yeh ek element ke andar doosre elements ko target karta hai.
  ```css
  div p { color: blue; }
  ```

#### **Definition**:
CSS Selectors patterns hote hain jo elements ko select karne ke liye use hote hain. Common selectors hain **Universal Selector, Type Selector, Class Selector, ID Selector, Attribute Selector, aur Descendant Selector**, jo alag-alag tarike se elements ko target karte hain.

---

### **5. Pseudo-classes and Pseudo-elements**

**Pseudo-classes** aur **pseudo-elements** special selectors hain jo specific conditions ya states ko target karte hain.

- **Pseudo-classes**: Yeh elements ke states ko target karte hain, jaise hover, active, visited, etc.
  ```css
  a:hover { color: red; }
  ```

- **Pseudo-elements**: Yeh kisi element ke specific part ko style karte hain, jaise first line, first letter, before, after, etc.
  ```css
  p::first-line { font-weight: bold; }
  ```

#### **Definition**:
Pseudo-classes aur pseudo-elements special selectors hain. Pseudo-classes elements ke states ko target karte hain, jaise **:hover**, jab user mouse se kisi element par jata hai. Pseudo-elements specific parts ko style karte hain, jaise **::first-line** jo first line ko target karta hai.

---

### **6. Z-Index**

**Z-Index** property stacking order ko control karti hai. Yeh batata hai ki kaunsa element upar dikhai dega jab multiple elements overlap hote hain. Z-index sirf positioned elements (absolute, relative, fixed) par hi kaam karta hai. Higher z-index value ka matlab hai element upar hoga.

```css
.box1 { position: absolute; z-index: 1; }
.box2 { position: absolute; z-index: 2; }
```

#### **Definition**:
Z-Index property elements ke stacking order ko control karti hai. Yeh un elements ko upar ya neeche dikhata hai jab multiple elements overlap karte hain. Higher z-index value wale elements hamesha upar dikhai dete hain.

---

### **7. Media Queries**

**Media Queries** CSS ki woh feature hai jo responsive design ko enable karta hai. Yeh alag-alag devices aur screen sizes ke liye different styles apply karne mein madad karta hai.

```css
/* Mobile devices */
@media (max-width: 600px) {
    body { background-color: lightblue; }
}

/* Tablets */
@media (min-width: 601px) and (max-width: 1024px) {
    body { background-color: lightgreen; }
}

/* Desktops */
@media (min-width: 1025px) {
    body { background-color: lightyellow; }
}
```

#### **Definition**:
Media Queries CSS ka ek feature hai jo responsive design ko enable karta hai. Yeh alag-alag devices ke liye different styles apply karne mein madad karta hai, jisse website har screen size par acche se dikhai de.

---

Ab yeh sab concepts **English** mein bhi explain karte hain:

---

### **1. CSS3 (Cascading Style Sheets 3)**

**CSS3** stands for the third version of Cascading Style Sheets. It is used for styling web pages. CSS3 introduced many new features that enhance styling capabilities, such as:

- **Flexbox**: Used for aligning elements horizontally or vertically, allowing the creation of responsive layouts.
  
- **Grid Layout**: Helps manage complex layouts by using rows and columns.

- **Animations and Transitions**: Allows elements to animate smoothly, such as hover effects on buttons or sliding effects for divs.

- **Media Queries**: Used to make websites responsive, changing the layout and styling based on different devices.

#### **Definition (English)**:
CSS3 is an advanced styling language that helps design web pages. It includes new features like **Flexbox, Grid, Animations, and Media Queries**, which make websites more interactive and responsive.

---

### **2. Box Model**

The **Box Model** is a fundamental concept in CSS. Every HTML element is treated as a box, divided into four main parts:

- **Content**: The actual content of the element, like text or images.
  
- **Padding**: The space around the content, providing

 distance between the content and the border.

- **Border**: The outer edge of the element, which can be styled and sized.

- **Margin**: The space outside the box, creating distance between the element and others.

Understanding the Box Model is crucial as it controls the size and layout of elements.

#### **Definition (English)**:
The Box Model is a concept where every HTML element is viewed as a box. It consists of four parts: **Content, Padding, Border, and Margin**, which define the positioning and spacing of the element.

---

### **3. Different Ways to Include CSS in a Web Page**

There are three ways to include CSS in a web page:

1. **Inline CSS**: Used directly within the HTML element using the style attribute. It’s good for quick styling but challenging for maintenance.
   ```html
   <h1 style="color: red;">Hello World!</h1>
   ```

2. **Internal CSS**: Written inside the `<style>` tag in the `<head>` section of the HTML document. It’s useful when you want to apply styles to a single page.
   ```html
   <head>
       <style>
           h1 { color: blue; }
       </style>
   </head>
   ```

3. **External CSS**: A separate `.css` file linked in the `<head>` section of the HTML document. This is the best practice as it makes the code modular and maintainable.
   ```html
   <head>
       <link rel="stylesheet" href="styles.css">
   </head>
   ```

#### **Definition (English)**:
CSS can be included in a web page in three ways: **Inline CSS**, written inside the element; **Internal CSS**, written inside the `<style>` tag; and **External CSS**, linked from an external CSS file. External CSS is best practice as it makes code easier to maintain.

---

### **4. All Selectors in CSS**

CSS selectors are patterns used to select elements. Some common selectors include:

- **Universal Selector (`*`)**: Targets all elements.
  ```css
  * { margin: 0; padding: 0; }
  ```

- **Type Selector**: Targets specific HTML elements.
  ```css
  p { color: green; }
  ```

- **Class Selector (`.`)**: Targets elements with a specific class.
  ```css
  .myClass { font-size: 20px; }
  ```

- **ID Selector (`#`)**: Targets an element with a specific ID.
  ```css
  #myId { background-color: yellow; }
  ```

- **Attribute Selector**: Targets elements with specific attributes.
  ```css
  input[type="text"] { border: 1px solid black; }
  ```

- **Descendant Selector**: Targets elements inside another element.
  ```css
  div p { color: blue; }
  ```

#### **Definition (English)**:
CSS Selectors are patterns used to select elements. Common selectors include **Universal Selector, Type Selector, Class Selector, ID Selector, Attribute Selector, and Descendant Selector**, which target elements in various ways.

---

### **5. Pseudo-classes and Pseudo-elements**

**Pseudo-classes** and **pseudo-elements** are special selectors that target specific conditions or parts of an element.

- **Pseudo-classes**: Target the states of elements, such as hover, active, visited, etc.
  ```css
  a:hover { color: red; }
  ```

- **Pseudo-elements**: Style a specific part of an element, such as the first line, first letter, before, after, etc.
  ```css
  p::first-line { font-weight: bold; }
  ```

#### **Definition (English)**:
Pseudo-classes and pseudo-elements are special selectors. Pseudo-classes target the states of elements, like **:hover**, when a user hovers over an element. Pseudo-elements style specific parts of an element, like **::first-line**, which targets the first line of a paragraph.

---

### **6. Z-Index**

The **Z-Index** property controls the stacking order of elements. It determines which element appears on top when multiple elements overlap. Z-index only works on positioned elements (absolute, relative, fixed). A higher z-index value means the element will be on top.

```css
.box1 { position: absolute; z-index: 1; }
.box2 { position: absolute; z-index: 2; }
```

#### **Definition (English)**:
The Z-Index property controls the stacking order of elements. It determines which elements appear on top or bottom when multiple elements overlap. Higher z-index values indicate that elements will appear above others.

---

### **7. Media Queries**

**Media Queries** enable responsive design in CSS. They allow different styles to be applied based on various devices and screen sizes.

```css
/* Mobile devices */
@media (max-width: 600px) {
    body { background-color: lightblue; }
}

/* Tablets */
@media (min-width: 601px) and (max-width: 1024px) {
    body { background-color: lightgreen; }
}

/* Desktops */
@media (min-width: 1025px) {
    body { background-color: lightyellow; }
}
```

#### **Definition (English)**:
Media Queries are a feature of CSS that enable responsive design. They allow different styles to be applied for various devices, ensuring that the website looks good on any screen size.
