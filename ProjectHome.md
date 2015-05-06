<font color='red'><strong><em>This project no longer maintained, please use other alternatives like <a href='https://github.com/karacas/imgLiquid'>imgLiquid</a>!</em></strong></font>

---

# Resize & Crop #
Handy _jQuery plugin_ for **client-side** uniform resizing & cropping. Ideal for avatars and images with similar size (more different sizes—the bigger bandwidth overhead).

## Ideal use ##
You can use plugin for [example to transform profile pictures of Facebook users](http://resize-crop.galik.it/avatars.php) (profile avatars). They are similar in size but not the same, but if you want to show them in a grid you probably want them to be same height (or/and width).

See [example with cats](http://resize-crop.galik.it) to get better understanding what Resize & Crop can do for you.

---

**Example how Resize & Crop works:**

![http://resize-crop.googlecode.com/files/resize-and-crop.jpg](http://resize-crop.googlecode.com/files/resize-and-crop.jpg)

---

**Code example:**
```
<script src="js/jquery.resizecrop.js"></script>
<script>
  
  $(document).ready(function(){
    $('img').resizecrop({
      width:40,
      height:60,
      vertical:"top"
    });  
  });  

</script>
```

---

**Note:**

If the image looks awful in IE6-7 try to use this little CSS snippet for better Bicubic Scaling:
```
img { -ms-interpolation-mode: bicubic; }
```