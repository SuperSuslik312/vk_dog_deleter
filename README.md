## Инструкция
1. Перейти в раздел **управление сообществом/участники**
2. Нажать CTRL+SHIFT+J, вставить данный код в консоль
3. Вуаля, собачек больше нет
```js
let dogs = 0;
let num = parseInt(document.querySelector("#group_u_summary").textContent)/20;
for (let i = 0; i < num; i++) {
    GroupsEdit.uShowMore();
}
lis = document.querySelector("#group_u_rows_members").childNodes;
for (let i = 0; i < lis.length; i++) {
    if (lis[i]["firstElementChild"]["firstElementChild"]["firstElementChild"].src === "https://vk.com/images/deactivated_100.png?ava=1") {
        document.querySelector("#group_u_rows_members").childNodes[i].childNodes[3]["firstElementChild"].onclick();
        dogs++;
    }
}
alert(`Удалено собак: ${dogs}.`);
```
