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

to parent:
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


  # to make specific element visible when the parent display is none

    display: initial;

  # to get a sentence in one line

    white-space: nowrap;

  # Animation

  animation is just a journey from initial position to final position.

  creating animation and applying animation is two diff things.

  creation:
  @keyframes identifier {
    
}
  initial
  from{

    }
    final
    to{
        
    }

    apply:
    animation-name: ;

# to make the object stay at the pos where it ended
 
    animation-fill-mode: forwards;


# iteration 

    animation-iteration-count: infinite;
    
# direction

    animation-direction: alternate;

# animation timing graph

    animation-timing-function: ease-in-out;


# sudo elements - before and after

they come after or before the content of element and not the element itself.

# css bug

jab bhi parent div and child div create kia ho aur agar child div ko margin dete top se to uske saath parent div bhi khisak jata cux dono ek dusre ke saath ekdum close hai so usko solve krne ki liye parent ko top se padding deni padti and bug will be fixed.

# to blur bg

    backdrop-filter: blur(10px);

# to adjust text with background

/* mix-blend-mode: */

# to get the scrolling pics like marquee
    display: inline-block;
    white-space: nowrap;
    overflow-x: auto;
    overflow-y: hidden;
  
  @keyframes Scroll-Anime {
    from{
        transform: translate(0);
    }
    to{
        transform: translate(-100%);
    }
}
  
  # for hand on screen
    cursor: pointer;
  
  # to fit bg img in particular size

  background-fit: cover;

  # for stroke text

    -webkit-text-stroke: 2px black transparent;

# inline block me do elements ke bich ka gap 4 px hota

# to center an element:

    child -> 
    position: relative; (will adjust acc to parent)
    left: 50%;
    transform: translateX(-50%);

# to create scrollable elements on main axis
     
    to parent:
    display: flex;
    flex-wrap: nowrap; (to stop the flexing)

    to child:
    flex-shrink: 0; (child wont shrink/adjust acc to parent)

# to scroll from x axis instead of whole page

overflow-x : auto; (main axis me scrollbar/scroll)
overflow-y : hidden; (pura page scroll nahi hoga)

# inline-elements pe block ki properties like margin and padding do not work, therfore: we use inline-block property

# to create a scrollable elements using inline-block property:

parent -> white-space : nowrap; (isme jo bhi elements next line me 
                                 arhe the wo same line me ajate)

child -> display : inline-block; (to use features of both properties)

# for smoother transition of filter on an element

transition: filter 0.5s;

# for grayscale and blur other elements

    filter: grayscale(1) blur(5px);

# object fit: cover vs background size:cover

object fit: cover is used in img tag and bg size: cover is used in bg img

# to pause an animation when hover

.elem:hover .elem-slide{
    animation-play-state: paused!important;
}

# to add show to a box:

box-shadow: x-axis y-axis blur rgba(0, 0, 0, 0.400);
}

# to change pos of button 
{
  position: relative
  left:50%
  transform: translatex(-50%)
}