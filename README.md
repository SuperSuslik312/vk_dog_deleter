## Инструкция
1. Перейти в раздел **управление сообществом/участники**
2. Нажать CTRL+SHIFT+J, вставить данный код в консоль
3. Вуаля, собачек больше нет
```js
h = 0;
n = parseInt(parseInt(document.querySelector("#group_u_summary").textContent)/20);
while(h<n){
GroupsEdit.uShowMore();
h++
};
lis = document.querySelector("#group_u_rows_members").childNodes;
for (i=0;i<lis.length;i++){
if (lis[i]["firstElementChild"]["firstElementChild"]["firstElementChild"].src === "https://vk.com/images/deactivated_100.png"){
    document.querySelector("#group_u_rows_members").childNodes[i].childNodes[3]["firstElementChild"].onclick()
}
}
```
