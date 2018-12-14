---
layout: post
title: flag project v2
date: 2018-12-14
---
This week, we worked on coding our flags. It wasn't that hard but there was some parts that was hard. For example, when it came to coding the crecent that was in my flag. But some things that wasn't that hard was when it came to making the base of my flag and the big white strip on my flag. I am doing the Pakistan flag so there was a big white strip to the left of the flag. After making the base and white strip it then came to making the crecent and the star. The star wasn't that hard but the crecent was hard. I had to make 2 circles, which wasn't that hard, but the hard part was when it came to overlaying the two circles so it would look like a crecent. So I was just messing around with the overlaying and it took a while but I eventually got it to look almost or if not just like the Pakistan flag.
```;dimension of the flag 3:2
;colors of the flag white and forestgreen
;define
(define height 300)
(define width 200)
(define white-width (/ width 4))
(define flag(rectangle height width "solid" "forestgreen")) 
(define white(rectangle white-width 200 "solid" "white"))
(define asdf(put-image (rectangle 150 300 "solid" "white") 0 50 (rectangle height width "solid" "forestgreen")))
(define flagstar(rotate 100(star-polygon 20 5 2 "solid" "white")))
(define crecentShape (circle 50 "solid" "white"))
(define crecentShapeFill (circle 50 "solid" "forestgreen"))
crecentShape
(define crecentShapeWhole (put-image crecentShapeFill 50 75 crecentShape))
crecentShapeWhole
(define crecentShapeFinal (rotate -50 crecentShapeWhole))
(define flagBasew/Crecent (put-image crecentShapeFinal 185 100 asdf))
;put-image
(put-image (rectangle 150 300 "solid" "white") 0 50 (rectangle height width "solid" "forestgreen"))
(put-image crecentShapeFinal 185 100 asdf)
(put-image flagstar 215 125 flagBasew/Crecent)
;star for the flag
(star-polygon 20 5 2 "solid" "black")
;one test
crecentShapeWhole
;one random rotation
(rotate 100 flagstar)
```

![Flag of Pakistan](/Images/flagv2.png)

