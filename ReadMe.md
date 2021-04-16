## Keyframes starter code 

1. git clone https://github.com/mattkrebs2000/StickySmoothActiveNavBarCSS-SomeJS.git

2. cd into StickySmoothActiveNavBarCSS-SomeJS

3. Use Live Server to see the result of the "Example" code.

4. Click on the links at the top to see how the page works. 

5. (General Description of the assignment) This repository contains a quick example of how a Sticky Smooth Active NavBar is constructed. Your goal is to manipluate the code in challenge.html and challenge.css in such a way that it behaves just like the Example does. 

6. Pass in your saved github repository link. 

<script>
          
		  let div = document.querySelectorAll("div a");
        
        window.addEventListener("scroll", event => {
          
            let fromTop = window.scrollY+5;
        
          div.forEach(link => {
            let div = document.querySelector(link.hash);
        
            if (
              div.offsetTop <= fromTop &&
              div.offsetTop + div.offsetHeight > fromTop
            ) {
              link.classList.add("current");
            } else {
              link.classList.remove("current");
            }
          });
        });
</script>