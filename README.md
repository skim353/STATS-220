# STATS-220

##### project 1
##### create meme gif
library(magick)

### meme project
```r
kanye_meme <- image_read("https://i.pinimg.com/736x/47/f1/44/47f144b4bacbff242eaa3e236c6926fe.jpg") %>%
image_blank(width = 480, 
            height = 500, 
            color = "#FFFFFF") %>%
  image_annotate(text = "Me when I drink Coke Zero instead of regular Coke",
                 color = "#000000",
                 size = 35,
                 font = "Helvetica")
```
animation %>% image_write("my_animation.gif")
