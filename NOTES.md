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

-   click
    > `$("button").click(func1)`
-   css()
    > `$("#img").css('width', '100%')`
