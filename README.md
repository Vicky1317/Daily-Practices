# Daily-Practices
HCJ ALL.Html:- 
TASK-1
<style>
    .box{
        background-color: blue;
        width: 200px;
        height: 200px;
        transition: 2s;
    }
#widthmax{
 width: 700px;
}
</style>
<div class="box">

</div>

<button onclick="change()" style="text-align: center;">CHANGE COLOR</button>
<script>
    var box=document.querySelector(".box")
    function change()
    {
        
        box.setAttribute("id","widthmax")
    }
</script>
TASK-2
<input id="inputbox">
<button onclick="change()">btn</button>
<h1 id="result"></h1>
<script>
    var inputbox=document.getElementById("inputbox")
    var result=document.getElementById("result")
    function change()
    {
        result.textContent=inputbox.value
    }
</script> //click the button to display the content

<input id="inputbox" onkeyup="update()">
<h1 id="result"></h1>
<script>
    var inputbox=document.getElementById("inputbox")
    var result=document.getElementById("result")
    function update()
    {
        result.textContent=inputbox.value
    }
</script> //while we display the o/p from onkey changes...
TASK-3
<button onclick="update()">Add</button>
<h1 id="result"></h1>
<script>
    // select h1
    var h1=document.getElementById("result")
    function update()
    {
        //append is used for create a duplicate of Hello or anything
        h1.append("Hello")
    }
</script>
// Updated Code from Previous Code
<button onclick="update()">Add</button>
<div id="result"></div>
<script>
    // select h1
    var div=document.getElementById("result")
    function update()
    {
        // creste element is used for create a duplicate tag For ex(<h1></h1>)
        var listitem=document.createElement("h1")
        listitem.textContent="Hello" //(Hello(One by One))
        //append is used for create a duplicate of Element Hello or anything For Ex(Hello,Hello,HEllo)
        div.append(listitem)
    }
</script>
TASK-4
<button id="btn" onclick="changecolor()">Change Color</button>
<script>
    // change the button color
    var color=document.getElementById(".btn")
    function changecolor()
    {
      btn.style.backgroundColor="Red" 
    }
</script>
TASK-5
// when we click the button that convert to text
<h1 id="result">Name</h1>  
<button onclick="update(event)">Vicky</button>
<button onclick="update(event)">John</button>
<button onclick="update(event)">Hari</button>
<script>
var result=document.getElementById("result")
function update(event) // Event is new element from this code
{
result.textContent=(event.target.textContent)
}
</script>
TASK-6
// While we click the button the element will be Erased..
<h1 onclick="removeitem(event)">One</h1>
<h1 onclick="removeitem(event)">Two</h1>
<h1 onclick="removeitem(event)">Three</h1>
<h1 onclick="removeitem(event)">Four</h1>
<h1 onclick="removeitem(event)">Five</h1>
<h1 onclick="removeitem(event)">Six</h1>
<script>
    function removeitem(event)
    {
event.target.remove()
    }
</script>
TASK-7
// popup menu
<style>
    .overlay {
        background-color: black;
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0px;
        left: 0px;
        opacity: 0.8;
        z-index: 1;
        display: none;
    }

    .popupbox {
        background-color: white;
        color: black;
        width: 40%;
        position: absolute;
        padding: 20px;
        left: 30%;
        z-index: 3;
        border-radius: 10px;
        display: none;

    }
</style>
 <button onclick="show()">Show</button>
<div class="overlay"></div>
<div class="popupbox">
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde omnis aut praesentium quo ullam id similique
        laboriosam nobis consequatur hic, fuga aliquam molestiae voluptatem veritatis magnam assumenda, aspernatur
        corporis quasi.</p>
    <button onclick="none()">Close</button>
</div>
<script>
    var overlay = document.querySelector(".overlay")
    var popupbox = document.querySelector(".popupbox")
    function show() {
        overlay.style.display = "block"
        popupbox.style.display = "block"
    }
    function none() {
        overlay.style.display = "none"
        popupbox.style.display = "none"
    }
</script> 
//Without calling function on button simply use addEvent.Listener to function the element
<button id="btn">Show</button>
<script>
    var button = document.getElementById("btn")
    button.addEventListener("click", function () {
        alert("Hello")
    })
    button.addEventListener("mouseover", function () {
        alert("MouseOver")
    })
</script>


