**This course is on [youtube](https://www.youtube.com/watch?v=QhQ4m5g2fhA)**

# What is jQuery

![What is jQuery]()

# jQuery Selectors

-   used to find document elements, id, value and much more
-   based on CSS selectors
-   **jquery need `id` to be unique for each element**
-   multi-select
-   child selectors
    > `$(div > p).fadeToggle()`
-   first element
    > `$(p:first).fadeToggle()`  
    > **Doesn't work with `p:second`**
-   even or odd element, only influences even or odd number of elements
    > `$(p:even).fadeToggle()`

###### All selectors

![all](img/selectors_all.png)

# jQuery Events

-   `.click()`
    > `$("button").click(func1)`
-   `.css(attribute, value)`
    > `$("#img").css('width', '100%')`
-   `.ready()`
    > execute the code after the document has loaded. It may cause problems if you are without onload, because the code may use an element that is not loaded.
    > [.ready()](https://www.w3schools.com/jquery/event_ready.asp)
    ```js
    $(document).ready(function () {
        $("button").click(function () {
            $("p").slideToggle();
        });
    });
    ```
-   double click: `.dblclick(function)`
-   `.mouseenter(function)`
-   `.mouseleave(function)`
-   `.hover(function1, function2)`

# jQuery Efects

-   hide and show
    -   `.hide()` and `.hide(2000)`
    -   `.show()` and `.show(2000)`
    -   `.toggle()` and `.toggle(2000)`
-   fade-in and fade-out
    -   `.fadeIn(2000)`
    -   `.fadeOut(2000)`
    -   `.fadeToggle(2000)`
-   slide-up and slide-down
    -   `.slideUp(2000)`
    -   `.slideDown(2000)`
    -   `.slideToggle(2000)`
-   stop

    > `.stop()`

    > The jQuery stop() method is used to stop an animation or effect before it is finished. The stop() method works for all jQuery effect functions, including sliding, fading and custom animations.

-   `.animate({}, 2000)`

    > [.animate()](https://www.w3schools.com/jquery/eff_animate.asp)

    > Definition and Usage
    >
    > The animate() method performs a custom animation of a set of CSS properties.
    >
    > This method changes an element from one state to another with **CSS styles**. The CSS property value is changed gradually, to create an animated effect.
    >
    > Only numeric values can be animated (like "margin:30px"). String values cannot be animated (like "background-color:red"), except for the strings "show", "hide" and "toggle". These values allow hiding and showing the animated element.
    >
    > Tip: Use "+=" or "-=" for relative animations.

    ```js
    $("#btn").animate(
        { left: "150px", opacity: "1", height: "400px", width: "400px" },
        2000
    );
    $("#btn").animate(
        { left: "150px", opacity: "1", height: "400px", width: "400px" },
        "slow"
    );
    ```
