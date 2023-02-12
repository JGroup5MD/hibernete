Task: Voting_Hibernate
#Group5 (@zax_ma,@socnyi_fruct, @peter_podobed, @Vitaliy79Sv)
Приложение предназначено для проведения голосования. В данном приложении есть две номенации:

Артисты - можно проголосовать только за одного артиста.
Жанры - пожно проголосовать за от 3 до 5 жанров.

В приложении реализован функционал:
1. Странница приветствия: URL "/welcome"

2. Странница артистов:
  URL "/singer" На данной странице предусмотрено выполнения следующих действий:
  (GET/POST/PUT)http://host:port/WarFileName/singer
- просмотр  артистов (метод GET)
- добавление артистов (метод POST) и необходимо передать ключ "add"
- обновление артиста (метод PUT) и необходимо передать ключи "updateId" и "newName"
- удаление артиста по номеру id (метод DELETE) и необходимо передать ключи "deleteId"

3. Странница жанров:
  URL "/jenre" На данной странице предусмотрено выполнения следующих действий:
  (GET/POST/PUT)http://host:port/WarFileName/jenre
- просмотр жанров  (метод GET)
- добавление жанров (метод POST) и необходимо передать ключ "add"
- обновление жанров  (метод PUT) и необходимо передать ключи "updateId" и "newName"
- удаление жанра по номеру  id (метод DELETE) и необходимо передать ключи "deleteId"

4. Странница голосования.
  URL "/vote" На данной странице предусмотрено голосование. Необходимо указать следующие ключи:
  (POST)http://host:port/WarFileName/vote
- для голосования за артиста "singer" и указать id
- для  голосования за жанры "genre" и указать id
- добавление информации к голосу "message" и написать текст сообщения
- необходимо указать свой email для отправки информации об отправленном голосе "email". 
  После отправки голоса пользователь получает информацию о текущих результатах голосования

5. Странница результатов голосования.
   (GET)http://host:port/WarFileName/result
   На данной станице можно просмотреть текущие результаты голосования

