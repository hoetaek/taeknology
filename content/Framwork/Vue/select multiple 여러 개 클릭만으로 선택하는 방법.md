```js
document.addEventListener("DOMContentLoaded", function () {  
    const selectElement = document.getElementById("board")  
  
    selectElement.addEventListener("mousedown", function (event) {  
        event.preventDefault()  
  
        const originalScrollTop = selectElement.scrollTop  
        const clickedOption = event.target  
  
        if (clickedOption.tagName === "OPTION") {  
            clickedOption.selected = !clickedOption.selected  
        }  
  
        selectElement.focus()  
        setTimeout(() => {  
            selectElement.scrollTop = originalScrollTop  
        }, 0)  
  
        return false  
    })  
}