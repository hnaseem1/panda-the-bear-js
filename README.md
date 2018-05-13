# DOM Manipulation with Panda the Bear
[See assignment in Alexa.](https://alexa.bitmaker.co/wdi/67/assignments/2051/latest)

document.querySelector('img').src = 'http://www.sciencemag.org/sites/default/files/styles/inline__450w__no_aspect/public/panda_16x9.jpg?itok=8a0-7WSj'

img = document.querySelectorAll('img')
imgs[1].src = 'http://www.sciencemag.org/sites/default/files/styles/inline__450w__no_aspect/public/panda_16x9.jpg?itok=8a0-7WSj'

document.querySelector('.bio-info-value').innerText = 'Hasan'

document.querySelector('.info-title')

document.querySelectorAll('.info-title')[1].innerText = 'Unemployment'

document.querySelector('body').style.color = 'red'



highlightClass = document.querySelectorAll('.highlight')
highlightClass.forEach(function(item){item.style.color = 'blue'})

document.querySelectorAll('h1').forEach(function(t){t.style.fontFamily = 'monospace'})

document.querySelectorAll('.action-icon-bg').forEach(function(t){ t.style.backgroundColor = 'red'})

document.querySelector('#name').placeholder = 'identify yourself'

document.querySelector('#message').placeholder = 'state your business'

document.querySelector('#name').value = 'your nemesis'

document.querySelector('#email').value = 'koalathebear@gmail.com'

document.querySelector('#submit').value = 'End garde'

document.querySelector('#submit').disabled = true

var element = document.querySelector('ul')
element.parentNode.removeChild(element)
<!--
Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing. ---- Done

Select the heading that says "Panda the Bear" and change it to your own name. --- Done

Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) ---- Done

Change the colour of the body. -------- Done

Change the colour of each element using the highlight class. Use a for loop to do this. ---- Done

Change the font family of the h1 to 'monospace'. ---- Done

Find a way to select the round icons in the sidebar and then change their colour.  ------- Done

Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -------  Done

Change the placeholder attribute of the message field to "state your business". ----- Done

Give the name field a "value" attribute of "your nemesis". ------- Done

Change the value attribute of the email field to "koalathebear@gmail.com". ------- Done

Change the value of the submit button on the contact form to "En garde!". ------- Done

We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). ----- Done

We should help Panda protect their privacy by erasing their personal details from the sidebar. -->




PART 2


div = document.getElementById('time-travel')
div.parentNode.removeChild(time)


pikachu = document.getElementById('right-image').querySelector('img')
var pikachuClone = pikachu.cloneNode()
document.querySelector('.portfolio-container').appendChild(pikachuClone)


for(i = 0; i <= 10; i++) {
  document.querySelector('.portfolio-container').appendChild(pikachuClone)
}


var listItem = document.createElement('li');
<br>
var leftSpan = document.createElement('span');
<br>
var lastUpdated = document.createTextNode('Page last updated on');
<br>
leftSpan.appendChild(lastUpdated);
<br>
listItem.appendChild(leftSpan);
<br>
leftSpan.classList.add("bio-info-title");
<br>
listItem.classList.add('bio-info-item');
<br>
var rightSpan = document.createElement('span');
<br>
var date = document.createTextNode(new Date);
<br>
rightSpan.appendChild(date);
<br>
rightSpan.classList.add("bio-info-title");
<br>
listItem.appendChild(rightSpan);
<br>
document.querySelector('.bio-info').appendChild(listItem);
