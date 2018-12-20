---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of Pakistan by Matthew

## Describe your program

-   What country did you design for? The country that I designed for is the Pakistan flag.
-   What grade do you expect? I expected a 4 because I think that I put a lot of thought in to the project. I made the flag geometrically accurate, and I made the flag scaleable. By making my flag scaleable I can just change the flag's size with one button. 



## Current output

-   Insert an image that your program currently produces.

* * *

![Flag of Pakistan](/Images/flagv2.png)
* * *

## Describe your process.

-   What questions, strategies, help from peers or teacher, or thinking got you to this point? One question that I asked is how to get the exact colors for the green part of my flag. Mr. Allata then helped me by telling me to search up the flags rgb color. Some strategies that I had was to find an easy base that would cover most of my flag. So I choose green because my flag if mostly made up of green. BT then helped me when it came to one of the rotations that I didn't know how to do. He also helped me on the scaling part because I wasn't not sure on how to make my flag scaleable. But once he helped me on one part. I did the rest of the scaling.




## Explain your code.

-   Choose a significant part of your program (15 lines max) and paste it below. Do not insert your entire program here. 
```
(define size 1)

(define height (* size 300))
(define width (* size 200))
(define white-width (* size 50))
(define flag(rectangle height width "solid" "forestgreen")) 
(define white (rectangle white-width (* size 200) "solid" "white"))
(define asdf(put-image (rectangle (* size 150) (* size 300) "solid" "white") 0 (* size 50) (rectangle height width "solid" "forestgreen")))
(define flagstar(rotate 100(star-polygon (* size 20) 5 2 "solid" "white")))
(define crecentShape (circle (* size 50) "solid" "white"))
(define crecentShapeFill (circle (* size 50) "solid" "forestgreen"))
crecentShape
(define crecentShapeWhole (put-image crecentShapeFill (* size 50) (* size 75) crecentShape))
crecentShapeWhole
(define crecentShapeFinal (rotate -50 crecentShapeWhole))
```
-   Explain each argument in the code section. Everything here is just me defining all of the things that I will need in order to complete my flag. I didn't make the function and then defined it, I just made the function and the defining in the same line. I also did some rotations when I was doing the functions.
-   Tell us how it functions independently and within the whole program. Each part of the code has its own thing to do.  One can be doing something to make the white stripe that I have on the flag, while the other can be making the star that I also have on my flag.

* * *

```
(define size 1)

(define height (* size 300))
(define width (* size 200))
(define white-width (* size 50))
(define flag(rectangle height width "solid" "forestgreen")) 
(define white (rectangle white-width (* size 200) "solid" "white"))
(define asdf(put-image (rectangle (* size 150) (* size 300) "solid" "white") 0 (* size 50) (rectangle height width "solid" "forestgreen")))
(define flagstar(rotate 100(star-polygon (* size 20) 5 2 "solid" "white")))
(define crecentShape (circle (* size 50) "solid" "white"))
(define crecentShapeFill (circle (* size 50) "solid" "forestgreen"))
crecentShape
(define crecentShapeWhole (put-image crecentShapeFill (* size 50) (* size 75) crecentShape))
crecentShapeWhole
(define crecentShapeFinal (rotate -50 crecentShapeWhole))
```

* * *

-   Explain the code you posted by telling us about each argument. There is one define for size and that is to make my flag scaleable. The rest is just me defining everything else and other parts of my flag.
-   Then tell us how your code section fits into the whole. They all have something that they have to do and they are all important parts when it comes to making my flag.
 



## Program code

```
;dimension of the flag 3:2
;colors of the flag white and forestgreen
;define
(define size 1)

(define height (* size 300))
(define width (* size 200))
(define white-width (* size 50))
(define flag(rectangle height width "solid" "forestgreen")) 
(define white (rectangle white-width (* size 200) "solid" "white"))
(define asdf(put-image (rectangle (* size 150) (* size 300) "solid" "white") 0 (* size 50) (rectangle height width "solid" "forestgreen")))
(define flagstar(rotate 100(star-polygon (* size 20) 5 2 "solid" "white")))
(define crecentShape (circle (* size 50) "solid" "white"))
(define crecentShapeFill (circle (* size 50) "solid" "forestgreen"))
crecentShape
(define crecentShapeWhole (put-image crecentShapeFill (* size 50) (* size 75) crecentShape))
crecentShapeWhole
(define crecentShapeFinal (rotate -50 crecentShapeWhole))
(define flagBasew/Crecent (put-image crecentShapeFinal (* size 185) (* size 100) asdf))
;put-image
(put-image (rectangle (* size 150) (* size 300) "solid" "white") 0 (* size 50) (rectangle height width "solid" "forestgreen"))
(put-image crecentShapeFinal (* size 185) (* size 100) asdf)
(put-image flagstar (* size 215) (* size 125) flagBasew/Crecent)
;star for the flag
(star-polygon (* size 20) 5 2 "solid" "black")
;one test
crecentShapeWhole
;one random rotation
(rotate 100 flagstar)
```
