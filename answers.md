## part 1 ##

1a. var image = document.querySelector('img')
image.src = "https://placebear.com/400/400"

1b. var pic = document.querySelectorAll('#left-image')
pic.src = "https://placebear.com/325/255"
###

2. var title = document.querySelector('h1')
title.innerText = "Melina"

3. var title = document.querySelectorAll('h3')
title[1]
####

4. var body = document.querySelector('body')
body.style.color = "red"

5. var highlight = document.querySelector('.highlight')
highlight.style.color = "blue"

6. var h1 = document.querySelector('h1')
h1.style.fontFamily = "monospace"

7. var icon = document.querySelectorAll('.action-icon-bg')
icon.style.backgroundColor = "purple"
#### changed one without All, couldn't change both (cannot set property
  of undefined)

8. var el = document.querySelector('#name')
el.setAttribute("placeholder", "identify yourself")

9. var msg = document.querySelector('#message')
msg.setAttribute("placeholder", "state your business")

10. el.setAttribute("value", "your nemesis")

11. var mail = document.querySelector('#email')
mail.setAttribute("value", "koalathebear@gmail.com")

12. var button = document.querySelector('#submit')
button.setAttribute("value", "en garde!")

13. button.disabled = true;

14. var info = document.querySelector('form')
info.reset();

## part 2 ##

1a. skills = document.querySelectorAll('.bar-default')
skills = document.querySelectorAll('.bar-default')[2]
timetravel = document.querySelector('#time-travel')
skills.removeChild(timetravel)

1b. var pikachu = document.querySelector('#right-image')
pikachu.cloneNode
var container = document.querySelector('.portfolio-container')
container.appendChild(pikachu)
VM2082:1 Uncaught DOMException: Failed to execute 'appendChild' on 'Node': The new child element contains the parent.
    at <anonymous>:1:11
### but other way around doesn't have error (yet still doesnt work/clone)

2. for (var i=0; i < 10, i++) { var pikachu = document.querySelector('#left-image').cloneNode();
container.appendChild(pikachu); }
## syntax error (unexpected )

3.
var listItem = document.createElement('li');
var leftSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated);
listItem.appendChild(leftSpan);
var rightSpan = document.createElement('span');
var now = new Date();
var bioinfo = document.querySelector('.bio-info');
bioinfo.appendChild(leftSpan);
rightSpan.innerHTML = now
bioinfo.appendChild(rightSpan);
