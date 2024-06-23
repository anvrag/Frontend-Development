# div

BOX == DIV
jaha ek se jyada elements dikhe waha div hai.
jaha bhi rectangular shape dikhe wha bhi div hai.

ek box banao jo ki red ho
steps:
div banao html me
usse h and w do since it doesnt have height but has width
bgcolor : red

# for css:

<h1> </h1>
h1 or any tag name like
h1{}
it calls the tag

<h1 id="main">
# -> for id

<h1 class="red">
. -> for class

# for color and bg color:

color = text color
bgcolor = background color

# units - px % rem em vh vw max-height min-height max min width

1 area me jitne jaada pixels utna jyada sharp image or vid or graphics
and 1 area me jitne kam pixels utna kam sharp img or video or graphics
px - depends upon screen quality

% - jitna total hai uska hissa,also changes its shape acc to screen.
% hamesha apne parent se value leta hai eg: html,body
eg: 70 % w - total screen ka 70 % width

vw & vh : view port height and width and wo hamesha screen se value lete hai.

em (element): depends upon element ke font size par, aur ye parent ko dete hai to child pe bhi apply hota hai.
eg: ek element jiska font size is 16px to 1em ki value 16px hogi.
aur agar font size change hua to em ki val bhi change hogi.
it will be fixed like px

rem (root element): depends upon html ke font size par

1 rem = 16px

max & min : max ek max hook/limit/boundary laga deta and min ek min limit/boundary/hook laga deta
used for responsiveness.

# Font-Family : 2 types - san serif and serif

font-family:Playwrite Is;
font-weight: 500;
text-transform: capitalize;
text-decoration: line-through;

# Font-size: 40px; to change size of font.

            for responsiveness, use vw.

# Line-Height: to adjust the spacing between the lines.

# Text-allign: to adjust the position of the text.

               by default - it is left.
               justify - wont leave any space.

# Padding & Margin.

padding is to create imaginary border around the child which is inside the parent (div) and the padding is given to parent and not child. its like creating border inside the div

Margin is to create border outside of div or insert/apply space between two or more elements which can be inside the parent(div).

# Border

border: px;
border-color: ;
border-style: solid;
border-radius: ; use 50% for circle

# Display Properties

inline : inline is like uske baaju me koi bhi dusre elements ko allow krta hai but inline doesnt allow to change its height and width.

Block : Block is like uske baaju me koi bhi dusra elements ko allow NAHI krta hai. takes full space. can change height and width.

Inline-Block : mixture of above properties, agar inline ki height and width change krni ho to inline-block ke thru kr skte hai. using
display: inline-block; also a block element will behave like inline meaning it will allow elements uske baaju me.

# Position

Absolute : koi bhi element jiski pos is absolute wo upar uth jyega and uske niche/baju ke elements uske piche/niche chup jyenge.
hum kisi element ko bhi pos abso bana skte. to koi bhi uth jyega and by default elements are on 0 layer and jaise jiska numbering wo us layer pe uthega and jitna jyada num ka layer wo baaki uske kam layer ke elements ko overlap krdega.

Relative : agr koi element jo ki div k inside hai aur usse absolute krdia to wo to div ke bahar ja pyega aur agar hume usse restrict krna hai to we can use position: relative for that div so the element inside moves inside div only. so element will move w respect/relative to div and not screen.

fixed : to stick the div or element at one position.

# CSS background

background: url();
background: linear-gradient(direction (to right, to right bottom),color1,color2,color3);
background: color;

background-image : url(); isme linear-gradient bhi chlta but not in background-color.

background-size: cover; pure div me img ko cover
contain; img ko div me dalta chahe koi hissa chut
kyu na jye. it will repeat the img at
left over portion.
to no repeat -> background-repeat : no-repeat;

background-position: center/top/bottom/left/right;

# Flexbox

display : flex;

tab use hota when we want elements aaju baaju and want more control.
flexbox parent pe lagta hai not on child. flexbox ka nature hai ki child ek dusre ke side me ajate. flexbox se 2 axis activate hoti

1. y 2. x and ye parent pe hoti activate. y axis - cross , x axis - main. elements ki direction hame main axis batati hai. default me cross axis top se bottom jata hai.

main axis me work krne k liye use hota justify content.
cross axis me work krne k liye use hota align-items.

# CSS Psuedo-Elements

har element ke pass ek possibility hoti hai ki wo chahe to inactive 'After' AND 'Before' properties ko active kr ske.

::first-letter
::first-line (dynamic hota);
::selection (when a text is selected)

# Psuedo-Classes

:hover - text,img, so on..
:active - buttons
:focus - when focus on inputs
:nth-child(n) - to control any one element, like 5 paragraphs to control 3rd para we can use nth-child(3); to handle every third element use 3n .

# Color-Science

color-name : red , green.
hexadecimal-notation : #
RGB functional notation :rgb
RGBA functional notation :rgba - a - alpha(transperancy)

screen bani hai khoob sare leds se and ye leds 3 colors show kr skte
and unka combination bhi.

css me har color ki min value is 0 and max value is 255

red - 255
green - 255
blue - 255

teeno full intensity - white.
teeno low intensity - black.

# GRID

its need is for the perfect structure/layout of the website.

flexbox is a single dimensional property meaning hum elements ko sirf ek hi direction me target kr skte either rows or columns.
Grid is a two dimensioinal property meaning hum elements ko rows and columns dono direction me target kr skte or dono ko ek baar me handle kr skte .

#main {
height: 100%;
width: 100%;
background-color: lightblue;
/_ display: flex;
justify-content: space-between;
flex-direction: column-reverse;
align-items: center; _/
display: grid; /_ -> automatically elem ke H and W adjust kr liye _/
grid-template-columns: 200px 200px;
grid-template-rows: 200px 200px;
/_ align-items: center;
justify-items: center; _/
align-content: center;
justify-content: center;
}

.elem {
/_ height: 200px;
width: 200px; _/
background-color: crimson;
border: 2px black solid;
}

to justify a child - use justify-self : ;

to resize the specific element.
#eleme1 {
background-color: greenyellow;
grid-row: 1 / 3;
grid-column: 1 / 4;
}

# Gap

use gap to give gap between elements.

# opacity

to change the opacity of an element.

# for img tag

use object-fit : contain;

# to rotate element from -90 deg

#rotated {
position: absolute;
left: 10.5%;
bottom: 0;
rotate: -90deg;
transform-origin: 0 0;
color: azure;
font-weight: 400;
}

# to fit in one page without scrollbar

height: calc(100% - 150px); works with diff values

# to avoid the wrap done by using flexbox

use:

display: flex;
flex-wrap: nowrap;
flex-shrink: 0;

# for scrollbar on specific section or portion

  overflow-x: auto;

# to hide scrollbar

#text-content::-webkit-scrollbar {
    display:none;
}

# to change the style of scrollbar

#text-content::-webkit-scrollbar-thumb {
    /* display:none; */
    background-color: #f92526;
    border-radius: 8px;
}


# media - responsiveness

  (most smartphone comes within 600px)
 @media (max-width:600px) {
  
 }

 # fit-content

  height: fit-content; -> jitne line me content ban jaye