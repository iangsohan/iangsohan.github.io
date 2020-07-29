# iangsohan.com

## Introduction

[iangsohan.com](http://iangsohan.com/) is a personal website designed with HTML and JavaScript. The website is designed to be a quick and easy way to learn about my life, education, goals, and interests.

## Code Samples

"collapsible.js" - Collapsible Lists:
```
var coll = document.getElementsByClassName("collapsible");
var i;
for (i = 0; i < coll.length; i++) {
    coll[i].addEventListener("click", function() {
        this.classList.toggle("active");
        var content = this.nextElementSibling;
        if (content.style.maxHeight)
            content.style.maxHeight = null;
        else
            content.style.maxHeight = content.scrollHeight + "px";
    });
}
```
<br />

"contacts.js" - Contacts Dropdown:
```
function myFunction() {
    document.getElementById("myDropdown").classList.toggle("show");
}

window.onclick = function(event) {
    if (!event.target.matches('.contact') && !event.target.matches('.con-element')) {
        var dropdowns = document.getElementsByClassName("dropdown-content");
        var i;
        for (i = 0; i < dropdowns.length; i++) {
            var openDropdown = dropdowns[i];
            if (openDropdown.classList.contains('show'))
                openDropdown.classList.remove('show');
        }
    }
}
```

## Installation

1. Download All Files in [Website](https://github.com/iangsohan/Website) into the same folder
2. Click on "home.html"
3. Navigate as Directed

## License

[MIT](https://choosealicense.com/licenses/mit/)
