<!--
_________________________________________________________________________________
<script>
    let users = ['dimych', 'valera', 'artem', 'katya']

    yo();

    if (users.length > 4) {
        yo();
    } else {

    }

    if (users.length < 2 || window !== null) {
        yo()
    }

    for (let i=0;i<1;i++) {
        yo()
    }

    function yo(){}

</script> 3
____________________________________________________________________________
<script>
    const hello = () => { alert('hello') }
</script>

<script>
    function hello() { alert('hello') }
</script>
____________________________________________________________________________
<script>
    function removeWhitespaces(string) {
        string.split(' ').filter(s => s !== '').join('_')
    }

    console.log(removeWhitespaces('you are JS developer'))
</script> return
____________________________________________________________________________
<script>
    let skills = ['css', 'html', 'js'];
    skills.XXX('react');
</script> push
____________________________________________________________________________
<script>
    let user = {age: 0};
    for (let i = 0; i < 10; i++) {
        user.age = i;
    }
    console.log(user.age)
</script>9
____________________________________________________________________________
<script>
    let user = {
        name: 'samurai',
        age: 18
    }

    let user2 = user;

    user2.name = 'ninja';
    console.log(user.name)
</script> ninja
____________________________________________________________________________
<script>
    let user = {
        name: "samurai",
        age: 18
    }
    console.log(user.age)
</script>

<input id="search"/>
<button id="find">find</button>
____________________________________________________________________________
<script>
    const searchInputElement = document.getElementById('search')
    const huntButtonElement = document.getElementById('find')

    huntButtonElement.addEventListener('click', () => {
        console.log(searchInputElement.value)
    })

    /*
    Что нужно написать внутри скобок вместо XXX и YYY, чтобы при нажатии на кнопку увидеть текст, введённый в input?
    Ответ дайте через пробел.
    Пример ответа: firstword secondword
    */

</script>huntButtonElement 'click'
_____________________________________________________________________________
<input id="anxiety" value="it-incubator"/>

<script>
    const searchInputElement = document.querySelector('it-incubator');
    searchInputElement.value = '';

    /*
    Что нужно написать внутри скобок вместо XXX, чтобы значение в поле ввода зачищалось?
    */
</script>'#anxiety'
________________________________________________________________________________
<input id="latvia" value="it-incubator"/>

<script>
    const inputElement = document.getElementById('latvia');
    inputElement.value = '';

    /* Что нужно написать вместо XXX, чтобы значение в поле ввода зачищалось?
 В качестве ответа укажите строчку целиком.  */
</script> 

const inputElement = document.getElementById('latvia');
-->

-----------------------------------------------------------------------
<script>
    let user = {age: 0};
    for (let i = 0; i < 10; i++) {
        user.age = i;
    }
</script>

user.age = 9

<script>
    let user = {
        name: 'samurai',
        age: 18
    }

    let user2 = user;

    user2.name = 'ninja';
    console.log(user.name) ninja
</script>

<input id="search"/>
<button id="find">find</button>
-->

<script>
    const searchInputElement = document.getElementById('search')
    const lookButtonElement = document.getElementById('find')

    lookButtonElement.addEventListener('click', () => {
        console.log(searchInputElement.value)
    })

    /*
    Что нужно написать внутри скобок вместо XXX и YYY, чтобы при нажатии на кнопку увидеть текст, введённый в input?
    Ответ дайте через пробел.
    Пример ответа: firstword secondword
    */

</script>

________________________________________________ Monday week 1 _________________________________________________________
export const Wrapper  = () => {
return <Courage city="minsk" />
}
type PropsType = {
city: string
}
export const Courage: React.FC<PropsType> = (props) => {
return <div>hello</div>
}

/*
В коде в разных местах допущена одна и та же ошибка.
Какое слово должно быть написано вместо ошибочного?
*/

Courage
________________________________________________________________________________________________________________________
import ReactDOM from 'react-dom'

export const VideoBlock = () => {
return <div>
<VideoHeader />
<VideoContent />
<VideoStatistics />
</div>
}
export const VideoHeader = () => {
return <div>
😀 Заголовок видео
</div>
}
export const VideoContent = () => {
return <div>
📼 Контент видео
</div>
}
export const VideoStatistics = () => {
return <div>
📊 Статистика лайков
</div>
}

ReactDOM.render(<div>ххх</div>,
document.getElementById('root')
);

//Что нужно написать вместо ххх, чтобы на экране увидеть:
//😀 Заголовок видео
//📼 Контент видео
//📊 Статистика лайков
// ❗ Ответ дать минимально возможным объёмом кода
<VideoBlock/>
________________________________________________________________________________________________________________________
type UserPropsType = {
name: string
description: string
}
export const User: React.FC<UserPropsType> = (props) => {
return <div>
<h1>Имя: {props.name}</h1>
//<div>Описание: {ххх}</div>
</div>
}

//Что нужно написать вместо ххх, что бы код работал?

props.description
________________________________________________________________________________________________________________________
type PropsType = {
city: string        // 'minsk'
country: string     // 'belarus'
coords?: string     // '53.917501,27.604851'
}

export const Wrapper1 = () => {
return <PropsComponent1 city='minsk'/>
}

export const PropsComponent1: React.FC<PropsType> = (props) => {
return <div>hello</div>
}

// Что МИНИМАЛЬНО ДОСТАТОЧНО нужно дописать в строке 8 (cтрока с ошибкой), чтобы не было ошибки
country='belarus'
________________________________________________________________________________________________________________________
type PagePropsType = {
age: number
name: string
avatarUrl: string
}
const Page: React.FC<PagePropsType> = (props) => {
return <User a={xxx} n={yyy} />
}
type UserPropsType = {
a: number
n: string
}
export const User: React.FC<UserPropsType> = (props) => {
return <div>name: {props.n}, age: {props.a}</div>
}

// Что нужно написать вместо xxx и yyy?
// Ответ дайте через пробел, например: blabla onClick(props)
props.age props.name
________________________________________________________________________________________________________________________
type NewsType = {
title: string
author: string
}
type ArticleType = {
title: string
date: string
text: string
}
type PagePropsType = {
news: NewsType[]
mainArticle: ArticleType
}
export const Page: React.FC<PagePropsType> = (props) => {
return <div>
<article>
<h1>Название: {props.XXX.title}</h1>           
<div>{props.XXX.date}</div>
<div>{props.XXX.text}</div>
</article>
<aside>Articles:
<ul>
{props.YYY.map(n => <li>{n.title}, {n.author}</li>)}
</ul>
</aside>
</div>
}
mainArticle news
________________________________________________________________________________________________________________________
type UserWalletType = {
    title: string
    amount: number
}
type UserWalletPropsType = {
    wallet: UserWalletType
}

export const UserWallet: React.FC<UserWalletPropsType> = (props) => {
return <div>title: {props.wallet.title}, amount: {props.wallet.amount}</div>
}

export const UserMoney = () => {
const wallets = [
{title: 'bitcoin', amount: 1},
{title: '$', amount: 100}
]

    return <div>
        <UserWallet wallet={xxx} />
        <UserWallet wallet={yyy} />
    </div>
}
wallets[0]
wallets[1]
________________________________________________________________________________________________________________________
import ReactDOM from 'react-dom'

export const VideoHeader = (props: {videoName: string}) => {
return <div>
😀 {props.videoName}
</div>
}
export const VideoContent = (props: {videoContent: string}) => {
return <div>
📼 <a href={props.videoContent}>{props.videoContent}</a>
</div>
}
export const VideoDescription = (props: {videoDescription: string}) => {
return <div>
📑 {props.videoDescription}
</div>
}

export const YoutubeVideo = (props: any) => {
return <div>
<VideoHeader videoName={props.video.title} />
<VideoContent videoContent={props.video.link} />
<VideoDescription videoDescription={props.video.description} />
</div>
}

export const App = () => {
const video = {
title: 'Samurai way',
link: 'https://www.youtube.com/watch?v=gb7gMluAeao&list=PLcvhF2Wqh7DNVy1OCUpG3i5lyxyBWhGZ8',
description: 'Best free react-course'
}

    return <YoutubeVideo video={video} />
}

ReactDOM.render(<App />,
document.getElementById('root')
);
________________________________________________________________________________________________________________________
import ReactDOM from 'react-dom'

const Son = (props: any) => {
return <div>
I am son. My name is {props.name}
</div>
}


const Father = (props: any) => {
return <div>
I am father. My name is {props.name}
<Son name={props.sonName} />
</div>
}

const Granny = (props: any) => {
return <div>
I am granny. My name is {props.name}
<Father name={props.fatherName} sonName={props.sonName} />
</div>
}

export const App = () => {
return <div>
<Granny XXX={'Бабуля'} YYY={'Батя'} ZZZ={'Сын'}/>
</div>
}

ReactDOM.render(<App/>,
document.getElementById('root')
)
name
fatherName
sonName
________________________________________________________________________________________________________________________
import ReactDOM from 'react-dom'

const CrazyButton = (props: any) => {

    const style = {
        color: props.XXX,
        backgroundColor: props.YYY
    }

    return <button style={style}>
        {props.ZZZ}
    </button>
}

export const App = () => {
return <div>
<CrazyButton title={'delete'} fontColor={'white'} bgColor={'red'}/>
<CrazyButton title={'add'} fontColor={'white'} bgColor={'green'}/>
</div>
}

ReactDOM.render(<App/>,
document.getElementById('root')
)


___________________________________________ Monday Week 3_______________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

function User(props: UserType) {
return (
<li>Student {props.name}: {props.age} y.o.</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 34},
{id: 2, name: "Alex", age: 29},
{id: 3, name: "Ann", age: 25},
{id: 4, name: "John", age: 36},
]
const [users, setUsers] = useState<Array<UserType>>(data)
return (
<main>
<h4>User list:</h4>
<ul>
{/*{*/}
{/*    users.map(u => <User xxx={u.id}*/}
{/*                         id={u.id}*/}
{/*                         name={u.name}*/}
{/*                         age={u.age}*/}
{/*        />*/}
{/*    )*/}
{/*}*/}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо xxx, чтобы код работал оптимально?
________________________________________________________________________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

function User(props: UserType) {
return (
<li>Student {props.name}: {props.age} y.o.</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 34},
{id: 2, name: "Alex", age: 29},
{id: 3, name: "Ann", age: 25},
{id: 4, name: "John", age: 36},
]
const [users, setUsers] = useState<Array<UserType>>(data)
return (
<main>
<h4>User list:</h4>
<ul>
{/*{ users.map(u => <User key={u.id} {...xxx} />) }*/}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо xxx, чтобы код работал?

id={u.id} name={u.name} age={u.age}

________________________________________________________________________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

function User(props: UserType) {
return (
<li>User {props.name}: {props.age} y.o.</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
// Пользователи старше 25 лет:
// const olderThen25Users = users.xxx(u => u.age > 25)
return (
<main>
<h4>User list:</h4>
<ul>
{/*{ olderThen25Users.map(u => <User key={u.id} {...u}/>)}*/}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо xxx, чтобы код работал?

________________________________________________________________________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

function User(props: UserType) {
return (
<li>User {props.name}: {props.age} y.o.</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
// Необходимо отрендерить список пользователей старше 25 лет:
// const getOlderThen25Users = (u: xxx) => u.age > 25
// const olderThen25Users = users.filter(getOlderThen25Users)
return (
<main>
<h4>User list:</h4>
<ul>
{/*{ olderThen25Users.map(u => <User key={u.id} {...u}/>)}*/}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);

// Что надо написать вместо xxx, чтобы код работал?
________________________________________________________________________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

function User(props: UserType) {
return (
<li>User {props.name}: {props.age} y.o.</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
// Необходимо отрендерить список ользователей старше 25 лет:
const getOlderThen25Users = (u: UserType) => u.age > 25
const olderThen25Users = users.filter(getOlderThen25Users)
return (
<main>
<h4>User list:</h4>
<ul>
{ olderThen25Users.map(u => <User key={u.id} {...u}/>)}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что вернёт выражение: Array.isArray(olderThen25Users)
________________________________________________________________________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

type UserPropsType = UserType & {
deleteUser: (id: number) => void
}

function User(props: UserPropsType) {
const deleteUser = () => props.deleteUser(props.id)
return (
<li>
<button onClick={deleteUser}>x</button>
User {props.name}: {props.age} y.o.
</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
const deleteUser = (userID: number) => {
const filteredUsers = users.filter(u => u.id !== userID)
// setUsers(xxx)
}
return (
<main>
<h4>User list:</h4>
<ul>
{users.map(u => <User
key={u.id}
{...u}
deleteUser={deleteUser}
/>)}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо xxx, чтобы код работал?
________________________________________________________________________________________________________________________
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Button() {
return <button
// onClick={xxx}
>Click</button>
}


ReactDOM.render(
<Button/>, document.getElementById('root')
);





// Что надо написать вместо ххх,
// что бы на странице появился пустой alert при клике по кнопке?
________________________________________________________________________________________________________________________
import React, {MouseEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Button() {
const onClickHandler = (e: MouseEvent<HTMLButtonElement>) => {
// console.log((typeof e) === ххх)
}
return <button onClick={onClickHandler} >Click</button>
}


ReactDOM.render(
<Button/>, document.getElementById('root')
);

// Какой тип данных представляет аргумент функции-обработчика?
// Что надо написать вместо ххх, что бы в консоль вывело true?
________________________________________________________________________________________________________________________
import React, {useState, MouseEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Button() {
const [tagName, setTagName] = useState<string>()
const onClickHandler = (e: MouseEvent<HTMLButtonElement>) => {
// setTagName(e.xxx.tagName)
}
return (
<>
<p>{tagName}</p>
<button onClick={onClickHandler} >
<span>Click</span>
</button>
</>
)
}

ReactDOM.render(
<Button/>, document.getElementById('root')
);

// Что надо написать вместо ххх, что бы на странице появился текст BUTTON?
________________________________________________________________________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

type UserPropsType = UserType & {
deleteUser: (id: any) => void
}

function User(props: UserPropsType) {
return (
<li>
<button onClick={()=>props.deleteUser(props.id)}>x</button>
User {props.name}: {props.age} y.o.
</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
const deleteUser = (userID: number) => {
setUsers(users.filter(u => u.id !== userID))
}
return (
<main>
<h4>Users list:</h4>
<ul>
{users.map(u => <User
key={u.id}
{...u}
deleteUser={deleteUser}
/>)}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// В типе UserPropsType у функции deleteUser в параметрах указан тип "any".
// Какой тип было бы указать правильнее?
________________________________________________________________________________________________________________________

                                            
_______________________________________________ Monday week 4 __________________________________________________________

import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

type UserPropsType = UserType & {
deleteUser: (id: number) => void
}

function User(props: UserPropsType) {
return (
<li>
{/*<button onClick={() => props.deleteUser(xxx)}>x</button>*/}
User {props.name}: {props.age} y.o.
</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
const deleteUser = (userID: number) => {
const filteredUsers = users.filter(u => u.id !== userID)
setUsers(filteredUsers)
}
return (
<main>
<h4>User list:</h4>
<ul>
{users.map(u => <User
key={u.id}
{...u}
deleteUser={deleteUser}
/>)}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо xxx, чтобы код работал?
props.id

_________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

type UserPropsType = UserType & {
deleteUser: (id: number) => void
}

function User(props: UserPropsType) {
const deleteUser = () => props.deleteUser(props.id)
return (
<li>
{/*<button onClick={xxx}>Delete</button>*/}
User {props.name}: {props.age} y.o.
</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
const deleteUser = (userID: number) => {
const updatedUsers = users.filter(u => u.id !== userID)
setUsers(updatedUsers)
}
return (
<main>
<h4>User list:</h4>
<ul>
{users.map(u => <User
key={u.id}
{...u}
deleteUser={deleteUser}
/>)}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);

// Что надо написать вместо xxx, чтобы код работал?

() => props.deleteUser(props.id) wrong version

deleteUser - i think this is the right version
____

import React, {useState, MouseEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Post() {
const onClickHandler = (e: MouseEvent<HTMLAnchorElement>) => {
// xxx
alert("Летим-бомбим!!!")
}
return (
<div>
<article>
<h4>Как дела, братан?</h4>
<p>
Вижу, что неплохо. Давай, трудись )))
Google ждёт тебя в цифровом рабстве!
Cтавь лайк и полетели!!!
</p>
<a href={"https://www.youtube.com/"}
onClick={onClickHandler}
>В этом месте подробнее...</a>
</article>
</div>
)
}

ReactDOM.render(
<Post/>, document.getElementById('root')
);
// Что надо написать вместо ххх, чтобы Вас не направило на страницу Youtube
// при клике по ссылке?

e.preventDefault()

------------------------------------------------------------
import React, {useState, MouseEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function AuthForm() {
const onClickHandler = (e: MouseEvent<HTMLButtonElement>) => {
// xxx
alert()
}
return (
<form>
<div>
<label style={{padding: "10px 0"}}>
Name:
<input type={"email"} name={"email"}/>
</label>
</div>
<div>
<label style={{padding: "10px 0"}}>
Password:
<input type={"password"} name={"password"}/>
</label>
</div>
<button
onClick={onClickHandler}
type={"submit"}>
Log in
</button>
</form>
)
}

ReactDOM.render(
<AuthForm/>, document.getElementById('root')
);
// Что надо написать вместо ххх, чтобы данные из формы
// не отправлялись на сервер и страница не перезагружалась
// при клике по кнопке?
e.preventDefault()
________________________________________________________________________________________________________________________


import React, {useState, MouseEvent, ChangeEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function User() {
const [userName, setUserName] = useState<string>("")
// const onChangeHandler = (e: xxx )=> setUserName(e.currentTarget.value)
return (
<div>
<p>{userName}</p>
<input
// onChange={onChangeHandler}
/>
</div>
)
}

ReactDOM.render(
<User/>, document.getElementById('root')
);
// Что надо написать вместо ххх, чтобы правильно типизировать
// параметр функции?
ChangeEvent<HTMLInputElement>
________________________________________________________________________________________________________________________


import React, {useState, MouseEvent, ChangeEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function User() {
const [userName, setUserName] = useState<string>("")
return (
<div>
<p>{userName}</p>
<input
// xxx
onChange={(e) => setUserName(e.currentTarget.value)}
/>
</div>
)
}

ReactDOM.render(
<User/>, document.getElementById('root')
);
// Что надо написать вместо ххх, чтобы инпут был контролируемым?

value={userName}
________________________________________________________________________________________________________________________
import React, {useState, MouseEvent, ChangeEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function User() {
const [userName, setUserName] = useState<string>("")
const [text, setText] = useState<string>("")
const onChangeHandler = (e: ChangeEvent<HTMLInputElement> )=> setUserName(e.currentTarget.value)
return (
<div>
<input
value={userName}
onChange={onChangeHandler}
onBlur={()=> {
// xxx
setText(userName)
}}
/>
<p>{text}</p>
</div>
)
}

ReactDOM.render(
<User/>, document.getElementById('root')
);
// Что надо написать вместо ххх,
// чтобы после вывода текста в параграф содержимое формы ввода очищалось?

setUserName('')
________________________________________________________________________________________________________________________
import React, {useState, MouseEvent, ChangeEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Notes() {
const [newNote, setNewNote] = useState<string>("")
const [notes, setNotes] = useState<Array<string>>([])
const onChangeHandler = (e: ChangeEvent<HTMLTextAreaElement> )=>
setNewNote(e.currentTarget.value)
const addNote = () => {
setNotes([newNote, ...notes])
setNewNote("")
}
return (
<div>
<textarea
value={newNote}
onChange={onChangeHandler}
// xxx = {addNote}
/>
<h4>Notes:</h4>
<div>
{notes.map((n,i )=> <p key={i}>{n}</p>)}
</div>
</div>
)
}


ReactDOM.render(
<Notes/>, document.getElementById('root')
);
// Что надо написать вместо ххх,
// чтобы при потере инпутом фокуса добавлялась заметка?

onBlur
________________________________________________________________________________________________________________________

import React, {useState, MouseEvent, ChangeEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Notes() {
const [newNote, setNewNote] = useState<string>("")
const [notes, setNotes] = useState<Array<string>>([])
const onChangeHandler = (e: ChangeEvent<HTMLTextAreaElement> )=>
setNewNote(e.currentTarget.value)
const addNote = () => {
setNotes([newNote, ...notes])
setNewNote("")
}
return (
<div>
<textarea
value={newNote}
onChange={onChangeHandler}
onBlur={addNote}
/>
<div>
<button
// onClick={xxx}
>Clear notes list</button>
</div>
<h4>Notes:</h4>
<div>
{notes.map(n => <p>{n}</p>)}
</div>
</div>
)
}

ReactDOM.render(
<Notes/>, document.getElementById('root')
);
// Что надо написать вместо ххх,
// чтобы при клике список заметок очищался?

() => setNotes([])

________________________________________________________________________________________________________________________
Итоговый

type UserPropsType = {
name: string
description: string
}
export const User: React.FC<UserPropsType> = (props) => {
return <div>
<h1>Имя: {props.name}</h1>
//<div>Описание: {ххх}</div>
</div>
}

//Что нужно написать вместо ххх, что бы код работал?

import ReactDOM from 'react-dom'

const Son = (props: any) => {
return <div>
I am son. My name is {props.name}
</div>
}


const Father = (props: any) => {
return <div>
I am father. My name is {props.name}
<Son name={props.sonName} />
</div>
}

const Granny = (props: any) => {
return <div>
I am granny. My name is {props.name}
<Father name={props.fatherName} sonName={props.sonName} />
</div>
}

export const App = () => {
return <div>
<Granny XXX={'Бабуля'} YYY={'Батя'} ZZZ={'Сын'}/>
</div>
}

ReactDOM.render(<App/>,
document.getElementById('root')
)


import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function UsersList() {
const results = useState<Array<string>>(["Bob", "Alex", "Ann"])

    const users = results[0]
    const setUsers = results[1]

    return (
       <p>Тут будет список пользователей</p>
    )
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);

// Чему равно results.length?




import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function UsersList() {
const [users, setUsers] = useState<Array<string>>(["Bob", "Alex", "Ann"])
return (
<p>Тут будет список пользователей</p>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что вернёт выражение: typeof setUsers?


import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

function User(props: UserType) {
return (
<li>User {props.name}: {props.age} y.o.</li>
)
}

function UsersList() {
const state = [
{id: 1, name: "Bob", age: 34},
{id: 2, name: "Alex", age: 25},
{id: 3, name: "Ann", age: 30},
{id: 4, name: "John", age: 23},
]
const users = [
{id: 1, userName: "Bob", age: 34},
{id: 2, userName: "Alex", age: 25},
{id: 3, userName: "Ann", age: 30},
{id: 4, userName: "John", age: 23},
]

    const [usersList, setUsersList] = useState<Array<UserType>>(XXX)
    return (
        <main>
            <h5>User list:</h5>
            <p>Тут будет список пользователей</p>
        </main>
    )
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо XXX, чтобы код работал?
// ❗ Если мы отмапим массив, то должны увидеть данные пользователей
// ❗ Ответ дать минимально возможным объёмом кода

import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

function User(props: UserType) {
return (
<li>User {props.name}: {props.age} y.o.</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
// Пользователи старше 25 лет:
// const olderThen25Users = users.xxx(u => u.age > 25)
return (
<main>
<h4>User list:</h4>
<ul>
{/*{ olderThen25Users.map(u => <User key={u.id} {...u}/>)}*/}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо xxx, чтобы код работал?

import React, {MouseEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Button() {
const onClickHandler = (e: MouseEvent<HTMLButtonElement>) => {
// console.log((typeof e) === ххх)
}
return <button onClick={onClickHandler} >Click</button>
}


ReactDOM.render(
<Button/>, document.getElementById('root')
);

// Какой тип данных представляет аргумент функции-обработчика?
// Что надо написать вместо ххх, что бы в консоль вывело true?

import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
age: number
}

type UserPropsType = UserType & {
deleteUser: (id: number) => void
}

function User(props: UserPropsType) {
return (
<li>
<button onClick={() => props.deleteUser(xxx)}>x</button>
User {props.name}: {props.age} y.o.
</li>
)
}

function UsersList() {
const data: Array<UserType> = [
{id: 1, name: "Bob", age: 25},
{id: 2, name: "Alex", age: 28},
{id: 3, name: "Ann", age: 23},
{id: 4, name: "John", age: 30},
]
const [users, setUsers] = useState<Array<UserType>>(data)
const deleteUser = (userID: number) => {
const filteredUsers = users.filter(u => u.id !== userID)
setUsers(filteredUsers)
}
return (
<main>
<h4>User list:</h4>
<ul>
{users.map(u => <User
key={u.id}
{...u}
deleteUser={deleteUser}
/>)}
</ul>
</main>
)
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо написать вместо xxx, чтобы код работал?

import React, {useState, MouseEvent, ChangeEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function User() {
const [userName, setUserName] = useState<string>("")
return (
<div>
<p>{userName}</p>
<input
// xxx
onChange={(e) => setUserName(e.currentTarget.value)}
/>
</div>
)
}

ReactDOM.render(
<User/>, document.getElementById('root')
);
// Что надо написать вместо ххх, чтобы инпут был контролируемым?


import React, {useState, MouseEvent, ChangeEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Notes() {
const [newNote, setNewNote] = useState<string>("")
const [notes, setNotes] = useState<Array<string>>([])
const onChangeHandler = (e: ChangeEvent<HTMLTextAreaElement> )=>
setNewNote(e.currentTarget.value)
const addNote = () => {
setNotes([newNote, ...notes])
setNewNote("")
}
return (
<div>
<textarea
value={newNote}
onChange={onChangeHandler}
onBlur={addNote}
/>
<div>
<button
// onClick={xxx}
>Clear notes list</button>
</div>
<h4>Notes:</h4>
<div>
{notes.map(n => <p>{n}</p>)}
</div>
</div>
)
}

ReactDOM.render(
<Notes/>, document.getElementById('root')
);
// Что надо написать вместо ххх,
// чтобы при клике список заметок очищался?







_____________________________________________________________________ tuesday week 1 ___________________________________

import React, {useState, MouseEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function ColorButton() {
const [isColored, setIsColored] = useState<boolean>(false)
return (
<button
style={{ backgroundColor: `${ isColored === true ? "red": ""}`}}
onClick={()=>setIsColored(true)}
>
Меняю цвет по клику
</button>
)
}


ReactDOM.render(
<ColorButton/>, document.getElementById('root')
);

// Что надо написать вместо XXX, чтобы при клике кнопка становилась красной? 

isColored

import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function PasswordChecker() {
const [password, setPassword] = useState<string>("")
return (
<main>
<p>Your password must have more than 8 charters!</p>
<input
placeholder={"Enter your password"}
value={password}
onChange={e => setPassword(e.currentTarget.value)}
type={"password"}
/>
{XXX < 9 && <p style={{color: "red"}}>The password is too short!</p>}
</main>
)
}

ReactDOM.render(
<PasswordChecker/>, document.getElementById('root')
);

// Что надо вставить вместо XXX, чтобы код работал нормально? password.length

import React, { ChangeEvent, useState } from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function LongCommentChecker() {
const minSizeComment = 5
const [isCommentReady, setIsCommentReady] = useState<boolean>(false)
const [comment, setComment] = useState<string>('')

    const onClickSendComment = () => {
        if (comment.length > minSizeComment) {
            setComment('')
        }
    }
    const onChangeHandler = (e: ChangeEvent<HTMLTextAreaElement>) => {
        const newComment = e.currentTarget.value
        if (newComment.length > minSizeComment) {
            setIsCommentReady(true)
        } else {
            setIsCommentReady(false)
        }
        setComment(newComment)
    }

    return (
        <main>
            <textarea
                placeholder={'Your comment must have more than 5 charters'}
                value={comment}
                onChange={onChangeHandler}
            />
            <div>
                <button
                    disabled={XXX}
                    onClick={onClickSendComment}>
                    Send comment
                </button>
            </div>
        </main>
    )
}

ReactDOM.render(<LongCommentChecker/>, document.getElementById('root'));

// Что нужно написать вместо XXX, чтобы кнопка отправки комментария отрабатывала верно:
// первоначально кнопка должна быть в состоянии disable, а после успешного выполнения условия
// (комментарий должен быть больше 5 символов) должна раздизаблиться.
// ❗ Ответ необходимо дать на основании данных (переменных), которые уже есть в коде !isCommentReady

import React, {ChangeEvent, useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Colorize() {

const [color, setColor] = useState<string>("black")
const colors = ["red", "yellow", "green", "blue", "violet", "chartreuse"]

const styles = {
width: "100px",
height: "100px",
borderRadius: "50%",
backgroundColor: "black"
}

const getColor = (colors: string[]) => {
const nextColor = colors[Math.floor(Math.random() * colors.length)]
return nextColor
}

return (
<main>
<div style={{...styles, backgroundColor: color}}/>
<div>
<button
onClick={() => setColor(XXX)}
>
Get random color
</button>
</div>
</main>
)
}

ReactDOM.render(
<Colorize/>, document.getElementById('root')
);
// Что надо вставить вместо XXX, чтобы круг менял цвет по клику? getColor(colors)

import React, { ChangeEvent, useState } from 'react';
import ReactDOM from 'react-dom';
import './index.css';

type UserType = {
id: number
name: string
personalData: PersonalDataType
}
type PersonalDataType = {
gender: string
age: number
technologies: Array<TechnologiesType>
}
type TechnologiesType = 'HTML' | 'CSS' | 'React' | 'JS/TS' | 'Redux'

function UsersList() {

    const [users, setUsers] = useState<Array<UserType>>([
        {
            id: 1,
            name: 'Bob',
            personalData: {
                gender: 'male',
                age: 23,
                technologies: ['HTML', 'CSS', 'React', 'JS/TS', 'Redux']
            }
        },
        {
            id: 2,
            name: 'Alex',
            personalData: {
                gender: 'male',
                age: 21,
                technologies: ['HTML', 'CSS', 'React']
            }
        },
        {
            id: 3,
            name: 'Ann',
            personalData: {
                gender: 'female',
                age: 26,
                technologies: ['HTML', 'CSS', 'JS/TS']
            }
        },
        {
            id: 4,
            name: 'Helen',
            personalData: {
                gender: 'female',
                age: 31,
                technologies: ['HTML', 'CSS']
            }
        },
        {
            id: 5,
            name: 'Donald',
            personalData: {
                gender: 'male',
                age: 28,
                technologies: ['React', 'JS/TS', 'Redux']
            }
        },
    ])


    return <ul>
        {users.map(u => {
            return (
                u.XXX.length >= 5
                    ? <li key={u.id}>
                        {`User ${u.name}. ${u.personalData.age}. Ready to work.`}
                    </li>
                    : <li key={u.id}>
                        {`User ${u.name}. ${u.personalData.age}. `}
                    </li>)
        })}
    </ul>
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Те пользователи, у которых в стэке пять и более технологий, должны в списке
// быть отмечены, как готовые к работе.
// Что надо вставить вместо XXX, чтобы код работал нормально?  personalData.technologies
________________________________________________________________________________________________________________________