# HELLO
**I'm Kirill Avramov**  
Learn Front-End.  
From personal experience there is few pages with css animated elements and one JS App which you can see in my GitHub.  
As examples of code, I can give a couple of functions from my ToDO app.  

```javascript
//This function сhecks the message for validity and add it in List.
    function addToDo(){
        if (!(addMassage.value === '') && isNotExist(addMassage.value)) {
            let newTodo = {
                todo: addMassage.value,
                checked: false,
                important: false
            };
        
            todoList.push(newTodo);
            displayMessages();
            localStorage.setItem('todo', JSON.stringify(todoList));
            addMassage.value = '';
        }
    }
    
//update list when called from fuctions that chanch main list.    
    function displayMessages(){
    let displayMessage = ''
    todoList.forEach(function(item, i){
        displayMessage += `
        <li class='${item.important ? 'important' : ''}'>
            <input type="checkbox" name="" id='item_${i}' ${item.checked ? 'checked' : ''}>
            <label for='item_${i}'>${item.todo}</label>
        </li>
        `;
    })
    todo.innerHTML = displayMessage;
}
```

In terms of English, I understand well by ear, I am good at reading non-fiction literature (textbooks, documentation, articles on various topics). Bad at sentence composition and grammar. Really love English.
