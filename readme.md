# Dom Manipulation Assignment

# 1. Webiste Name: [Dev To](https://dev.to/)

### Toimages/Pics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./images/Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./images/Pic2.png)


### Code
```javascript
const sidebarCard = document.querySelector(".side-bar .crayons-card");

const title = sidebarCard.querySelector(".crayons-subtitle-2").innerHTML = "Dhruvil";

const passion = sidebarCard.querySelector("p");

passion.innerHTML = "I Create products, design & code them 💙";
```

### Result
![result1](./result/result1.png)

# 2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./images/Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']


### Code
```javascript
const devicesElements = document.querySelector(".as-imagegrid .row");

const deviceChildren = devicesElements.children;

const devicesArr = [];

for (const device of deviceChildren) {
    const deviceName = device.getElementsByTagName("a")[0].getAttribute("data-analytics-link-component_name");
    devicesArr.push(deviceName);
}

console.log(devicesArr);
```

### Result
![result2](./result/result2.png)


# 3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Toimages/Pics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./images/Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./images/Pic5.png)


### Code
```javascript
const accordian = document.querySelector(".accordion-homepage");

const newFaQ = document.createElement("section")
newFaQ.setAttribute("class", "parent")

const faqContent = document.createElement("h3")
faqContent.innerText = "My New FAQ"
faqContent.setAttribute("role", "button")
faqContent.setAttribute("aria-label", "My New FAQ")

newFaQ.appendChild(faqContent)

accordian.appendChild(newFaQ)
```


# 4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Toimages/Pics

     Query Selector, InnerText

### Sample Image

![Sample One](./images/Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./images/Pic7.png)

### Code
```javascript
const telephoneEl = document.querySelector(".one-tel-number")

telephoneEl.innerText = "+91 1234567890";
telephoneEl.setAttribute("href", "tel:+91 1234567890")
```

# 5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Toimages/Pics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./images/Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./images/Pic9.png)

### Code
```javascript
const checkoutElements = document.querySelectorAll(".feature-column-carousel__button .cta")

for(let checkoutElement of checkoutElements) {
    checkoutElement.innerText = "Check out"
}
```

# 6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Toimages/Pics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./images/Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./images/Pic11.png)


### Code
```javascript
const searchInputElement = document.querySelector(".searchinput___zXLAR")

searchInputElement.addEventListener('mouseover', function (){
    searchInputElement.style.backgroundColor = "red";
});
```


# 7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Toimages/Pics

       Form, Value, Submit

### Sample Image

![Sample One](./images/Pic12.png)

### Tasks

     To Search a toimages/Pic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./images/Pic13.png)


### Code
```javascript
const searchValue = "CSS Positions";

// search input
const searchInputElement = document.getElementById("hp-search-input");
searchInputElement.value = searchValue;

// submit button
const searchFormElement = document.querySelector("#hp-search-form")

searchFormElement.submit();
```


# 8. Webiste Name: [Google](https://www.google.com/)

### Toimages/Pics

       Remove Elements

### Sample Image

![Sample One](./images/Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./images/Pic15.png)


### Code
```javascript
const languagesListContainerElement = document.getElementById("SIvCob");

const languagesListElement = document.querySelectorAll("#SIvCob a");

languagesListElement.forEach((v, i)=>{
    let index = i + 1;

    // remove odd element
    if(index % 2 !== 0) {
        languagesListContainerElement.removeChild(v);
    }
})
```

# 9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Toimages/Pics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./images/Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./images/Pic17.png)

### Code
```javascript
const headingElement = document.querySelector("h1.display-heading-1");

headingElement.style.fontFamily = "monospace";
headingElement.style.color = "red";
```


# 10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Toimages/Pics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./images/Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./images/Pic19.png)


### Code
```javascript
const signupBtnElement = document.querySelector(".signup-btn.btn-cta-big");

const btnTextElement = signupBtnElement.querySelector(".signup-btn.btn-cta-big .login-btn-text")

signupBtnElement.addEventListener("mouseover", function(){
    btnTextElement.style.backgroundColor = "red";
});
```


# 11. Webiste Name: [realme](https://www.realme.com/in/)

### Toimages/Pics

       querySelector,style,background-image

### Sample Image

![Sample One](./images/Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./images/Pic21.png)


### Code
```javascript
const iNeuronLogo = "https://ineuron.ai/images/ineuron-logo.png";

const logoElement = document.querySelector("a.logo.gtag .icon-logo")

logoElement.style.backgroundImage = `url(${iNeuronLogo})`;
```


# 12. Webiste Name: [Github](https://github.com/)

### Toimages/Pics

       querySelector,style,background-Color

### Sample Image

![Sample One](./images/Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./images/Pic23.png)

### Code
```javascript
const btnElement = document.querySelector(".js-repos-container a");

btnElement.style.backgroundColor = "blue";
```

# 13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Toimages/Pics

       querySelector,innerHtml

### Sample Image

![Sample One](./images/Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./images/Pic25.png)


### Code
```javascript
document.querySelector(".fl-heading-text").innerHTML = "JSBOOTCAMP"
```


# 14. Webiste Name: [Asus](https://www.asus.com/in/)

### Toimages/Pics

      querySelector,style,font-size

### Sample Image

![Sample One](./images/Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./images/Pic27.png)

### Code
```javascript
document.querySelector(".HotDealsAll__Heading__2fIbe").style.fontSize = "80px";
```

# 15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Toimages/Pics

      querySelector,style.textAlign

### Sample Image

![Sample One](./images/Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./images/Pic29.png)

### Code
```javascript
const productG15LaptopCardElement = document.querySelector("#d560824win9b");

const productTitleElement = productG15LaptopCardElement.querySelector(".ps-top .ps-title")

productTitleElement.style.textAlign = "right";
```

# 16. Webiste Name: [Vercel](https://vercel.com/)

### Toimages/Pics

     querySelector,innerHTMl

### Sample Image

![Sample One](./images/Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./images/Pic31.png)

### Code
```javascript
document.querySelector(".section-title_title__VEDfK").innerHTML = "Start with Scratch";
```

# 17. Webiste Name: [Sony](https://www.sony.co.in/)

### Toimages/Pics

    querySelector,innerHTMl

### Sample Image

![Sample One](./images/Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./images/Pic32.png)


### Code
```javascript
document.querySelector(".btn.buy.buy-button").innerHTML = new Date().toString();
```


# 18. Webiste Name: [Philips](https://www.philips.co.in/)

### Toimages/Pics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./images/Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./images/Pic35.png)

### Code
```javascript
document.querySelector(".p-f03-footer-container").style.background = "orange";
```


# 19. Webiste Name: [Canon](https://in.canon/)

### Toimages/Pics

          querySelector,src

### Sample Image

![Sample One](./images/Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./images/Pic37.png)

### Code
```javascript
document.querySelector(".logo").getAttribute("src");
```

# 20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Toimages/Pics

          querySelector,style,color

### Sample Image

![Sample One](./images/Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./images/Pic39.png)

### Code
```javascript
document.querySelector(".wide h3.desc").style.color = "orange";
```