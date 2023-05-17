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

</script> 
/* Сколько раз вызывается функция yo*/
____________________________________________________________________________

<script>
    function hello() { alert('hello') }
</script>

/* Перепишите функцию в стрелочном виде */
____________________________________________________________________________
<script>
    function removeWhitespaces(string) {
        string.split(' ').filter(s => s !== '').join('_')
    }

    
</script> 
/* Что нужно минимально дописать чтобы функция работала */
____________________________________________________________________________
<script>
    let skills = ['css', 'html', 'js'];
    skills.XXX('react');
</script> 
____________________________________________________________________________
<script>
    let user = {age: 0};
    for (let i = 0; i < 10; i++) {
        user.age = i;
    }
    
</script>

чему равно user.age
____________________________________________________________________________
<script>
    let user = {
        name: 'samurai',
        age: 18
    }

    let user2 = user;

    user2.name = 'ninja';
   
</script> 
/* Чему равно  user.name */
____________________________________________________________________________
<script>
    let user = {
        name: "samurai",
        age: 18
    }
    
</script>

<input id="search"/>
<button id="find">find</button>
/* чему равно user.age*/
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

</script>huntButtonElement 
_____________________________________________________________________________
<input id="anxiety" value="it-incubator"/>

<script>
    const searchInputElement = document.querySelector('it-incubator');
    searchInputElement.value = '';

    /*
    Что нужно написать внутри скобок вместо XXX, чтобы значение в поле ввода зачищалось?
    */
</script>
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

чему равно свойство user.age
-----------------------------------------------------------------------------
<script>
    let user = {
        name: 'samurai',
        age: 18
    }

    let user2 = user;

    user2.name = 'ninja';
   // чему равно свойство user.name
</script>

<input id="search"/>
<button id="find">find</button>


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
___________________________________________________Tuesday 2____________________________________________________________
type StudentType = {
id: number
name: string
}

type FriendsType = {
[key: string]: Array<string>
}

export const students: Array<StudentType> = [
{id: 1, name: "Bob"},
{id: 2, name: "Alex"},
{id: 3, name: "Ann"},
{id: 4, name: "Charley"},
]

export const friends: FriendsType = {
1: ["Oliver", "Jack", "Oscar",],
2: ["Jack", "Lewis", "Thomas",],
3: ["William", "Michael", "Lewis",],
4: ["Oscar", "James", "William",],
}

//Дан список студентов и структура,
//которая содержит список друзей каждого из студентов.
//Id студента является ключом к массиву его друзей.
//Какое значение лежит тут:  friends[3][1]? 
"Thomas"
________________________________________________________________________________________________________________________
type StudentType = {
id: number
name: string
}

type FriendsType = {
[key: string]: Array<String>
}

export const students: Array<StudentType> = [
{id: 1, name: "Bob"},
{id: 2, name: "Alex"},
{id: 3, name: "Ann"},
{id: 4, name: "Charley"},
]

export const friends: FriendsType = {
1: ["Oliver", "Jack", "Oscar",],
2: ["Jack", "Lewis", "Thomas",],
3: ["William", "Michael", "Lewis",],
4: ["Oscar", "James", "William",],
}

//Дан список студентов и структура,
//которая содержит список друзей каждого из студентов.
//Id студента является ключом к массиву его друзей.
//Какое значение лежит тут: friends[students[0].id][3]?

________________________________________________________________________________________________________________________
import React, {useState} from "react";

type samuraiType = {
id: string
name: string
status: "online" | "offline"
}
type CourseNameType = "HTML"|"JS"|"React"|"Redux"|"HomeWorks"
type CourseType = {
name: CourseNameType
mentor: string
isDone: boolean
}
type TechnologiesType = {
[userID: string]: Array<CourseType>
}

const samuraiID_1 = "64jf-87kg"
const samuraiID_2 = "90lg-34ks"
const samuraiID_3 = "12jm-05fd"

export const samurai: Array<samuraiType> = [
{id: samuraiID_1, name: "Bob", status: "online"},
{id: samuraiID_2, name: "Alex", status: "offline"},
{id: samuraiID_3, name: "Ann", status: "offline"},
]

export const technologies: TechnologiesType = {
[samuraiID_1]: [
{name: "HTML", mentor: "Svetlana", isDone: true},
{name: "JS", mentor: "Viktor", isDone: true},
{name: "React", mentor: "Dmitrij", isDone: false},
{name: "Redux", mentor: "Valera", isDone: false},
{name: "HomeWorks", mentor: "Ignat", isDone: true},
],
[samuraiID_2]: [
{name: "HTML", mentor: "Svetlana", isDone: true},
{name: "JS", mentor: "Viktor", isDone: true},
{name: "React", mentor: "Dmitrij", isDone: true},
{name: "Redux", mentor: "Valera", isDone: false},
{name: "HomeWorks", mentor: "Ignat", isDone: true},
],
[samuraiID_3]: [
{name: "HTML", mentor: "Svetlana", isDone: true},
{name: "JS", mentor: "Viktor", isDone: true},
{name: "React", mentor: "Dmitrij", isDone: false},
{name: "Redux", mentor: "Valera", isDone: false},
{name: "HomeWorks", mentor: "Ignat", isDone: false},
],
}

export const updateCourseStatus = (samuraiID: string, name: CourseNameType, isDone: boolean) => {
return {...technologies,
[samuraiID]: technologies[xxx].map(c => c.name === name ? {...c, isDone} : c)
}
}
// Дан список самураев из инкубатора и структура, хранящая данные о курсах,
// которые самурай уже прошёл, а так же о тех курсах, которые ему ещё предстоит пройти.
// Так же дана функция updateCourseStatus,
// которая позволяет отметить курс как пройденный самураем или снять такую отметку
// Что надо написать вместо XXX, чтобы функция работала?

_______________________________________________Tuesday 3________________________________________________________________
type StudentType = {
id: number
name: string
}

type FriendsType = {
[key: string]: Array<string>
}

export const students: Array<StudentType> = [
{id: 1, name: "Bob"},
{id: 2, name: "Alex"},
{id: 3, name: "Ann"},
{id: 4, name: "Charley"},
]

export const friends: FriendsType = {
1: ["Oliver", "Jack", "Oscar",],
2: ["Jack", "Lewis", "Thomas",],
3: ["William", "Michael", "Lewis",],
4: ["Oscar", "James", "William",],
}

const getMutualFriends = (st_1: StudentType, st_2: StudentType,) => {
const result: Array<string> = []
friends[st_1.id].forEach(f => friends[xxx].includes(f)? result.push(f): null)
return result
}

//Дан массив студентов и структура,
//которая содержит список друзей каждого из студентов.
// Так же дана функция  getMutualFriends, проверяющая наличие общих друзей
// у двух выбранных студентов.
//Функция принимает параметром два объекта типа StudentType
// и возвращает массив с именами общих друзей,
//если они есть и пустой массив, если таковых нету.
// Что надо написать вместо ххх, чтобы функция работала?

st_2.id
________________________________________________________________________________________________________________________

import React, {useState} from "react";

type UserType = {
id: number
name: string
status: "online" | "offline"
}

type AddressType = {
country: string
city: string
email: string
}

type AdressesType = {
[userID: string]: AddressType
}

const users: Array<UserType> = [
{id: 1, name: "Bob", status: "online"},
{id: 2, name: "Alex", status: "offline"},
{id: 3, name: "Ann", status: "offline"},
]

const addresses: AdressesType = {
1: {country: "Russia", city: "Moscow", email: "hey@email.com"},
2: {country: "Ukraine", city: "Kiev", email: "yo@send.ua"},
3: {country: "Belarus", city: "Minsk", email: "wow@gogo.ru"},

}

const updateUserAddress = (userID: number, key: string, newValue: string) => {
return {...addresses,
[userID]: {...addresses[xxx], [key]: newValue}
}
}
// Дан список пользователей и структура, хранящая адреса пользователей.
// Так же дана функция updateUserAddress,
// которая обновляет указанное в параметрах поле в адресе пользователя.
// Пример использования функции: updateUserAddress(2, "city", "Dnepropetrovsk")
// Что надо написать вместо ххх, чтобы функция работала корректно?

userID

________________________________________________________________________________________________________________________

import React, {useState} from "react";

type samuraiType = {
id: string
name: string
status: "online" | "offline"
}
type CourseNameType = "HTML"|"JS"|"React"|"Redux"|"HomeWorks"
type CourseType = {
name: CourseNameType
mentor: string
isDone: boolean
}
type TechnologiesType = {
[userID: string]: Array<CourseType>
}

const samuraiID_1 = "64jf-87kg"
const samuraiID_2 = "90lg-34ks"
const samuraiID_3 = "12jm-05fd"

export const samurai: Array<samuraiType> = [
{id: samuraiID_1, name: "Bob", status: "online"},
{id: samuraiID_2, name: "Alex", status: "offline"},
{id: samuraiID_3, name: "Ann", status: "offline"},
]

export const technologies: TechnologiesType = {
[samuraiID_1]: [
{name: "HTML", mentor: "Svetlana", isDone: true},
{name: "JS", mentor: "Viktor", isDone: true},
{name: "React", mentor: "Dmitrij", isDone: false},
{name: "Redux", mentor: "Valera", isDone: false},
{name: "HomeWorks", mentor: "Ignat", isDone: true},
],
[samuraiID_2]: [
{name: "HTML", mentor: "Svetlana", isDone: true},
{name: "JS", mentor: "Viktor", isDone: true},
{name: "React", mentor: "Dmitrij", isDone: true},
{name: "Redux", mentor: "Valera", isDone: false},
{name: "HomeWorks", mentor: "Ignat", isDone: true},
],
[samuraiID_3]: [
{name: "HTML", mentor: "Svetlana", isDone: true},
{name: "JS", mentor: "Viktor", isDone: true},
{name: "React", mentor: "Dmitrij", isDone: false},
{name: "Redux", mentor: "Valera", isDone: false},
{name: "HomeWorks", mentor: "Ignat", isDone: false},
],
}

export const updateCourseStatus = (samuraiID: string, name: CourseNameType, isDone: boolean) => {
return {...technologies,
[samuraiID]: technologies[xxx].map(c => c.name === name ? {...c, isDone} : c)
}
}
// Дан список самураев из инкубатора и структура, хранящая данные о курсах,
// которые самурай уже прошёл, а так же о тех курсах, которые ему ещё предстоит пройти.
// Так же дана функция updateCourseStatus,
// которая позволяет отметить курс как пройденный самураем или снять такую отметку
// Что надо написать вместо ххх, чтобы функция работала корректно?

samuraiID

________________________________________________________________________________________________________________________

import React, {useState} from "react";

type UserType = {
id: number
name: string
status: "online" | "offline"
}

type AddressType = {
country: string
city: string
email: string
}

type AdressesType = {
[userID: string]: AddressType
}


const users: Array<UserType> = [
{id: 1, name: "Bob", status: "online"},
{id: 2, name: "Alex", status: "offline"},
{id: 3, name: "Ann", status: "offline"},
]

export const addresses: AdressesType = {
1: {country: "Russia", city: "Moscow", email: "hey@email.com"},
2: {country: "Ukraine", city: "Kiev", email: "yo@send.ua"},
3: {country: "Belarus", city: "Minsk", email: "wow@gogo.ru"},

}

export const changeUserStatus = (userID: number, status: string) => {
console.log( users.xxx(u => u.id === userID ? {...u, status} : u))
}
changeUserStatus(2, "online")
// Дан список пользователей и структура, хранящая адреса пользователей.
// Так же дана функция changeUserStatus, которая меняет статус пользователя.
// Что надо написать вместо ххх, чтобы функция работала корректно?

map

________________________________________________________________________________________________________________________

type ActionType = {
type: "SUM"|"SUB"|"MULT"|"DIV"
payload: number
}

export const calculator = (state: number, action: ActionType) => {
switch (ХХХ) {
case "SUM":
return state + action.payload
case "SUB":
return state - action.payload
case "DIV":
return state / action.payload
default:
return state
}
}

//Что надо написать вместо ХХХ, чтобы функция calculator работала?


________________________________________________________________________________________________________________________

type ActionType = {
type: "SUM"|"SUB"|"MULT"|"DIV"
payload: number
}

export const calculator = (state: number, action: ActionType): number => {
switch (action.type) {
case "SUM":
return state + action.payload
case "SUB":
return state - action.payload
case "DIV":
return state / action.payload
default:
return state
}
}

//Обработка какого action.type не предусмотрена в функции calculator? "MULT"
________________________________________________________________________________________________________________________
type ActionType = {
type: "SUM"|"SUB"|"MULT"|"DIV"|"EXP"
payload: number
}

export const calculator = (state: number, action: ActionType): number => {
switch (action.type) {
case "SUM":
return state + action.payload
case "SUB":
return state - action.payload
case "DIV":
return state / action.payload
case "EXP":
return state ** action.payload
default:
return state
}
}

//Что вернёт такой вызов функции: calculator(10, {type: "MULT", payload: 2})?

________________________________________________________________________________________________________________________
type UserType = {
id: number
userName: string
email: string
password: string
}

type ChangeUserPasswordTypeAT = {
type: "CHANGE-USER-PASSWORD"
payload: {
XXX
YYY
}
}

export const userReducer =
(state: UserType[], action: ChangeUserPasswordTypeAT): UserType[] => {
switch (action.type) {
case "CHANGE-USER-PASSWORD":
return state.map(u =>
u.id === action.payload.id
? {...u, password: action.payload.newPassword}
: u)
default:
return state
}
}

//Какой код должен быть написан вместо XXX и YYY в типе //ChangeUserPasswordTypeAT, что бы редьюсер работал?
//В ответе напишите через пробел: XXX  YYY 
id: number newPassword: string
________________________________________________________________________________________________________________________
import React, {useState, MouseEvent} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function ColorButton() {
const [isColored, setIsColored] = useState<boolean>(false)
return (
<button
style={{ backgroundColor: `${ XXX === true ? "red": ""}`}}
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
________________________________________________________________________________________________________________________
import React, {useState} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function UsersList() {
const [users, setUsers] = useState<Array<string>>(["Bob", "Alex", "Ann"])
const getUser = (user: string, i: number) => <li key={i}>{user}</li>

    const usersList = (XXX === 0)
        ? <p>List is empty</p>
        :  <ul>
            { users.map(getUser)}
        </ul>

    return (
        <main>
            <button onClick={()=>setUsers([])}>Clear list</button>
            <h4>User list:</h4>
            {usersList}
        </main>
    )
}

ReactDOM.render(
<UsersList/>, document.getElementById('root')
);
// Что надо вставить вместо XXX, чтобы код корректно работал  со списком пользователей?
________________________________________________________________________________________________________________________
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

// Что надо вставить вместо XXX, чтобы код работал нормально?
________________________________________________________________________________________________________________________
type StudentType = {
id: number
name: string
}

type FriendsType = {
[key: string]: Array<String>
}

export const students: Array<StudentType> = [
{id: 1, name: "Bob"},
{id: 2, name: "Alex"},
{id: 3, name: "Ann"},
{id: 4, name: "Charley"},
]

export const friends: FriendsType = {
1: ["Oliver", "Jack", "Oscar",],
2: ["Jack", "Lewis", "Thomas",],
3: ["William", "Michael", "Lewis",],
4: ["Oscar", "James", "William",],
}

//Дан список студентов и структура,
//которая содержит список друзей каждого из студентов.
//Id студента является ключом к массиву его друзей.
//Какое значение лежит тут: friends[students[0].id][3]?
undefined
________________________________________________________________________________________________________________________
type StudentType = {
id: number
name: string
}

type FriendsType = {
[key: string]: Array<string>
}

export const students: Array<StudentType> = [
{id: 1, name: "Bob"},
{id: 2, name: "Alex"},
{id: 3, name: "Ann"},
{id: 4, name: "Charley"},
]

export const friends: FriendsType = {
1: ["Oliver", "Jack", "Oscar",],
2: ["Jack", "Lewis", "Thomas",],
3: ["William", "Michael", "Lewis",],
4: ["Oscar", "James", "William",],
}

const getMutualFriends = (st_1: StudentType, st_2: StudentType,) => {
const result: Array<string> = []
friends[st_1.id].forEach(f => friends[xxx].includes(f)? result.push(f): null)
return result
}

//Дан массив студентов и структура,
//которая содержит список друзей каждого из студентов.
// Так же дана функция  getMutualFriends, проверяющая наличие общих друзей
// у двух выбранных студентов.
//Функция принимает параметром два объекта типа StudentType
// и возвращает массив с именами общих друзей,
//если они есть и пустой массив, если таковых нету.
// Что надо написать вместо ххх, чтобы функция работала? st_2.id
________________________________________________________________________________________________________________________
import React, {useState} from "react";

type UserType = {
id: number
name: string
status: "online" | "offline"
}

type AddressType = {
country: string
city: string
email: string
}

type AdressesType = {
[userID: string]: AddressType
}

const users: Array<UserType> = [
{id: 1, name: "Bob", status: "online"},
{id: 2, name: "Alex", status: "offline"},
{id: 3, name: "Ann", status: "offline"},
]

const addresses: AdressesType = {
1: {country: "Russia", city: "Moscow", email: "hey@email.com"},
2: {country: "Ukraine", city: "Kiev", email: "yo@send.ua"},
3: {country: "Belarus", city: "Minsk", email: "wow@gogo.ru"},

}

const updateUserAddress = (userID: number, key: string, newValue: string) => {
return {...addresses,
[userID]: {...addresses[xxx], [key]: newValue}
}
}
// Дан список пользователей и структура, хранящая адреса пользователей.
// Так же дана функция updateUserAddress,
// которая обновляет указанное в параметрах поле в адресе пользователя.
// Пример использования функции: updateUserAddress(2, "city", "Dnepropetrovsk")
// Что надо написать вместо ххх, чтобы функция работала корректно?

________________________________________________________________________________________________________________________
type ActionType = {
type: "SUM"|"SUB"|"MULT"|"DIV"
payload: number
}

export const calculator = (state: number, action: ActionType): number => {
switch (action.type) {
case "SUM":
return state + action.payload
case "SUB":
return state - action.payload
case "DIV":
return state / action.payload
case "MULT":
return state * action.payload
default:
return state
}
}

const result = calculator(10, {XXX, payload: 5})
console.log(result)
//Что надо написать вместо XXX, что бы переменная result содержала значение 5?
________________________________________________________________________________________________________________________

type ActionType = {
type: "SUM"|"SUB"|"MULT"|"DIV"|"EXP"
payload: number
}

export const calculator = (state: number, action: ActionType): number => {
switch (action.type) {
case "SUM":
return state + action.payload
case "SUB":
return state - action.payload
case "DIV":
return state / action.payload
case "MULT":
return state * action.payload
case "EXP":
return state ** action.payload
default:
return state
}
}
const result = calculator(10, {XXX, payload: 0})
if (!(result - 1)){
console.log("IT-INCUBATOR")
}

//Что надо написать вместо XXX чтобы в консоли появилась строка "IT-INCUBATOR"?

________________________________________________________________________________________________________________________
type UserType = {
id: number
userName: string
email: string
password: string
}

type ChangeUserPasswordTypeAT = {
type: "CHANGE-USER-PASSWORD"
payload: {
XXX
YYY
}
}

export const userReducer =
(state: UserType[], action: ChangeUserPasswordTypeAT): UserType[] => {
switch (action.type) {
case "CHANGE-USER-PASSWORD":
return state.map(u =>
u.id === action.payload.id
? {...u, password: action.payload.newPassword}
: u)
default:
return state
}
}

//Какой код должен быть написан вместо XXX и YYY в типе //ChangeUserPasswordTypeAT, что бы редьюсер работал?
//В ответе напишите через пробел: XXX  YYY

____________________________________________Wednesday 1_________________________________________________________________
type Status = 'Stopped' | 'Playing' | 'Paused'
type StateType = {
volume: number // in percents
trackUrl: string // 'https://blabla.com/track01.mp3',
currentPlayPosition: number // milliseconds,
status: Status
}

export const playerReducer = (state: StateType, action: any) => {
switch (action.type) {
case XXX:
return {
...state,
trackUrl: action.url
}
default:
return state
}
}

const muteTrackAC = () => ({type: 'TRACK-MUTED'})
const changeTrackAC = (url: string) => ({type: 'TRACK-URL-CHANGED', url})
const changeTrackPlayStatusAC = (status: Status) => ({type: 'TRACK-STATUS-CHANGED', status})

//Какой тип должен быть вместо XXX?

'TRACK-URL-CHANGED'
________________________________________________________________________________________________________________________
type Status = 'Stopped' | 'Playing' | 'Paused'
type StateType = {
volume: number // in percents
trackUrl: string // 'https://blabla.com/track01.mp3',
currentPlayPosition: number // milliseconds,
status: Status
}
export const playerReducer = (state: StateType, action: any) => {
switch (action.type) {
case 'TRACK-STATUS-CHANGED':
return {
...state,
status: action.status
}
default:
return state
}
}

const muteTrackAC = () => ({type: 'TRACK-MUTED'})
const changeTrackAC = (url: string) => ({type: 'TRACK-URL-CHANGED', url})
const changeTrackPlayStatusAC = (status: Status) => ({type: 'TRACK-STATUS-CHANGED', status})

const state: StateType = {
status: 'Stopped',
currentPlayPosition: 1213,
trackUrl: 'https://blabla.com/track01.mp3',
volume: 100
}

const newState = playerReducer(state, XXX)
console.log(newState.status === 'Paused')

//Напишите вместо XXX правильный вызов правильного AC, чтобы в консоли было true

changeTrackPlayStatusAC('Paused')
________________________________________________________________________________________________________________________
type Status = 'Stopped' | 'Playing' | 'Paused'
type StateType = {
volume: number // in percents
trackUrl: string // 'https://blabla.com/track01.mp3',
currentPlayPosition: number // milliseconds,
status: Status
}
export const playerReducer = (state: StateType, action: any) => {
switch (action.type) {
case 'TRACK-VOLUME-CHANGED':
return {
...state,
XXX
}
default:
return state
}
}

const muteTrackAC = () => ({type: 'TRACK-MUTED'})
const changeVolumeAC = (volumeLevel: number) => ({type: 'TRACK-VOLUME-CHANGED', volumeLevel})
const changeTrackAC = (url: string) => ({type: 'TRACK-URL-CHANGED', url})
const changeTrackPlayStatusAC = (status: Status) => ({type: 'TRACK-STATUS-CHANGED', status})

const state: StateType = {
status: 'Stopped',
currentPlayPosition: 1213,
trackUrl: 'https://blabla.com/track01.mp3',
volume: 100
}
const newState = playerReducer(state, changeVolumeAC(20))
console.log(newState.volume === 20)

// Напишите вместо XXX правильную строку кода, чтобы изменить громкость трека и увидеть в консоли true.

volume: action.volumeLevel
________________________________________________________________________________________________________________________
export const reducer = (state: any, action: any) => {
switch (action.type) {
case 'TRACK-LIKED':
return {
...state,
[XXX]: {
...state[XXX],
likesCount: state[XXX].likesCount + 1
}
}
default:
return state
}
}

const likeTrackAC = (trackId: number) => ({type: 'TRACK-LIKED', trackId})


const state = {
12: {id: 12, likesCount: 10},
14: {id: 14, likesCount: 2},
100: {id: 100, likesCount: 0},
}
const newState = reducer(state, likeTrackAC(14))

console.log(newState[14].likesCount === 3)

// Что нужно написать вместо XXX, чтобы в консоли увидеть true?
// ❗ Захардкодженные значения использовать запрещено

action.trackId
________________________________________________________________________________________________________________________
export const reducer = (state: any, action: any) => {
switch (action.type) {
case 'TRACK-ADDED':
return XXX
default:
return state
}
}

const addTrackAC = (trackId: number) => ({type: 'TRACK-ADDED', trackId})


const state = [
{id: 12, likesCount: 10},
{id: 14, likesCount: 2},
{id: 100, likesCount: 0}
]
const newState = reducer(state, addTrackAC(300))

console.log(newState[3].likesCount === 0)

// Что нужно написать вместо XXX, чтобы трек корректно добавился и в консоли увидеть true?

[...state, {id: action.trackId, likesCount: 0}]
________________________________________________________________________________________________________________________
export const reducer = (state: any, action: any) => {
switch (action.type) {
case 'TRACK-DELETED':
return state.filter((track: any) => XXX)
default:
return state
}
}

const deleteTrackAC = (trackId: number) => ({type: 'TRACK-DELETED', trackId})


const state = [
{id: 12, likesCount: 10},
{id: 14, likesCount: 2},
{id: 100, likesCount: 0}
]
const newState = reducer(state, deleteTrackAC(14))

console.log(newState.length === 2)


// Что нужно написать вместо XXX, чтобы корректно удалить трек и в консоли увидеть true?

track.id !== action.trackId
________________________________________________________________________________________________________________________
type StateType = {
volume: number // in percents
trackUrl: string // 'https://blabla.com/track01.mp3',
currentPlayPosition: number // milliseconds,
}

export const reducer = (state: StateType, action: any) => {
switch (action.type) {
case XXX:
return {
...state,
trackUrl: action.url
}
case YYY:
return {
...state,
volume: 0
}
case ZZZ:
return {
...state,
currentPlayPosition: 0
}
default:
return state
}
}

const muteTrackAC = () => ({type: 'TRACK-MUTED'})
const changeTrackAC = (url: string) => ({type: 'TRACK-URL-CHANGED', url})
// перемотатьНаНачало:
const rewindToStart = () => ({type: 'TRACK-REWOUND-TO-START'})

// Какие типы должны быть вместо XXX, YYY и ZZZ?
// Ответ дать через пробел, например:   'BLABLA' 'HEYНЕY' 'HIPHOP'

'TRACK-URL-CHANGED' 'TRACK-MUTED' 'TRACK-REWOUND-TO-START'
________________________________________________________________________________________________________________________
import {combineReducers, createStore} from 'redux'

let initialState = {items: [{name: 'Dimych'}, {name: 'Ignat'}]}
const usersReducer = (state = initialState, action: any) => {
return state
}

const store = createStore(combineReducers({
users: usersReducer
}))

store.XXX(() => {
console.log('state changed')
})

store.dispatch({type: 'ANY'})

// Что нужно написать вместо XXX, чтобы в консоли увидеть 'state changed'?

subscribe
________________________________________________________________________________________________________________________
import {combineReducers, createStore} from 'redux'
import ReactDOM from 'react-dom'
import {Provider, useSelector} from 'react-redux'
import React from 'react'

let initialState = {items:
[
{id: 1, name: 'Dimych'},
{id: 2, name: 'Ignat'}
]
}
const usersReducer = (state = initialState, action: any) => {
return state
}

let authInitialState = {login: 'Margo', settings: {theme: 'dark'}}
const authReducer = (state = authInitialState, action: any) => {
return state
}

let rootReducer = combineReducers({
users: usersReducer,
auth: authReducer
})

const store = createStore(rootReducer)
type RootStateType = ReturnType<typeof rootReducer>

const selector = (state: RootStateType) => state.users.items

const Users = () => {

const users = XXX

    return <ul>
        {users.map(u => <li key={u.id}>{u.name}</li>)}
    </ul>
}

ReactDOM.render(<div>
<Provider store={store}>
<Users/>
</Provider>
</div>,
document.getElementById('root')
)

// Что нужно написать вместо XXX, чтобы отрендерить список юзеров?
// ❗ Ответ дать минимально возможным объёмом кода

useSelector(selector)
________________________________________________________________________________________________________________________

import React, {useState, useReducer, useEffect} from 'react';
import ReactDOM from 'react-dom';
import './index.css';

const changeCounter = (state: number, action: any): number => {
switch (action.type) {
case "INC_VALUE":
return state + 1
case "RESET":
return 0
case "DEC_VALUE":
return state - 1
default:
return state
}
}

function Counter() {
const [value, setValue] = XXX(changeCounter, 0)
const [isCounter, setIsCounter] = YYY(true)
const commonStyles: React.CSSProperties = {
border: "1px solid black",
margin: "100px auto",
width: "300px",
height: "150px",
textAlign: "center",
}
const btnStyles: React.CSSProperties = {
color: "white",
fontWeight: "bold",
backgroundColor: "darkgray",
borderRadius: "3px",
minWidth: "40px"
}

    return (
        <div style={commonStyles}>{
            isCounter
                ? <div >
                    <div style={{marginBottom: "20px"}}>
                        <h2>{value}</h2>
                        <button
                            style={{...btnStyles, backgroundColor: "red"}}
                            onClick={() => setIsCounter(false)}>OFF</button>
                    </div>
                    <button style={btnStyles} onClick={() => setValue({type: "INC_VALUE"})}>+</button>
                    <button style={btnStyles} onClick={() => setValue({type: "RESET"})}>0</button>
                    <button style={btnStyles} onClick={() => setValue({type: "DEC_VALUE"})}>-</button>

                </div>
                : <div style={{textAlign: "center"}}>
                    <h2>Counter not working</h2>
                    <button
                        style={{...btnStyles, backgroundColor: "green"}}
                        onClick={() => setIsCounter(true)}>ON</button>
                </div>
        }
        </div>
    )
}


ReactDOM.render(
<Counter/>, document.getElementById('root')
);
// Что надо написать вместо XXX и YYY, чтобы код работал? Напишите через пробел.

useReducer useState

________________________________________________________________________________________________________________________

import React from 'react'
import { createStore } from 'redux'
import { Provider, useSelector, useDispatch } from 'react-redux'
import ReactDOM from 'react-dom'

type StudentType = {
id: number
name: string
age: number
}

const initState = {
students:
[
{id: 1, name: 'Bob', age: 23},
{id: 2, name: 'Alex', age: 22}
] as Array<StudentType>
}
type AddStudentAT = {
type: 'ADD-STUDENT'
name: string
age: number
id: number
}

type InitialStateType = typeof initState

const studentsReducer = (state: InitialStateType = initState, action: AddStudentAT): InitialStateType => {
switch (action.type) {
case 'ADD-STUDENT':
return {
...state,
students: [...state.students, {
name: action.name,
age: action.age,
id: action.id
}]
}
}
return state
}

const appStore = createStore(studentsReducer)
type RootStateType = ReturnType<typeof studentsReducer>


const StudentList = () => {
const students = useSelector((state: RootStateType) => state.students)
return (
<ul>
{students.map(s => <li key={s.id}>{`${s.name}. ${s.age} years.`}</li>)}
</ul>
)
}
const App = () => {
return <StudentList/>
}

ReactDOM.render(<div>
<XXX YYY={ZZZ}>
<App/>
</XXX>
</div>,
document.getElementById('root')
)

// Что нужно написать вместо XXX, YYY и ZZZ, чтобы отобразился список студентов?

Provider store appStore
________________________________________________________________________________________________________________________

import {createStore} from 'redux'
import ReactDOM from 'react-dom'
import {Provider, useSelector, useDispatch} from 'react-redux'
import React from 'react'

const students = {
students: [
{id: 1, name: 'Bob'},
{id: 2, name: 'Alex'},
{id: 3, name: 'Donald'},
{id: 4, name: 'Ann'},
]
}
type RemoveStudentAT = {
type: "REMOVE-STUDENT"
id: number
}
const RemoveStudentAC = (id: number): RemoveStudentAT => ({
type: "REMOVE-STUDENT",
id
})

const studentsReducer = (state = students, action: RemoveStudentAT) => {
switch (action.type) {
case "REMOVE-STUDENT":
return {
...state,
students: state.students.filter(s => s.id !== action.id)
}
}
return state
}

const store = createStore(studentsReducer)
type RootStateType = ReturnType<typeof studentsReducer>


const StudentList = () => {
const listItemStyles = {
width: "100px",
borderBottom: "1px solid gray",
cursor: "pointer",
}
const students = useSelector((state: RootStateType) => state.students)
const dispatch = useDispatch()
const studentsList = students.map(s => {
const removeStudent = () => {
XXX(YYY( ZZZ))
}
return (
<li key={s.id}
style={listItemStyles}
onClick={removeStudent}>
{s.name}
</li>)
})
return (
<ol>
{studentsList}
</ol>

    )
}


ReactDOM.render(<div>
<Provider store={store}>
<StudentList/>
</Provider>
</div>,
document.getElementById('root')
)

// Что нужно написать вместо XXX, YYY и ZZZ, чтобы при клике по имени студент
// удалялся из списка? Напишите через пробел.

dispatch RemoveStudentAC s.id

_____________________________________________Wednesday_3________________________________________________________________
import React, { useState } from 'react'
import ReactDOM from 'react-dom'

export const TempManager = () => {
const [temp, setTemp] = useState(0)
const [seconds, setSeconds] = useState(0)

const resetTemp = () => setTemp(0)
const increaseSeconds = () => setSeconds(seconds + 100)

return (
<>
<TempDisplay temp={temp} reset={resetTemp}/>
<div>
<p><b>Секунды:</b> {seconds} с</p>
<button onClick={increaseSeconds}>
Увеличить время на 100 секунд
</button>
</div>
</>
)
}

const TempDisplay = React.memo((props: any) => {
console.log('Render TempDisplay')
return (
<div>
<p><b>Температура</b>: {props.temp} &#176;</p>
<button onClick={props.reset}>Reset</button>
</div>
)
})

ReactDOM.render(<TempManager/>, document.getElementById('root'))


//При увеличении времени (при клике на button) компонент TempDisplay
//тоже перерисовывается. Эта перерисовка является избыточной.
//Найдите в чем причина лишних перерисовок.
//Исправленную версию строки напишите в качестве ответа.

//Пример ответа: const increaseSeconds = () => setSeconds(seconds + 100)

const resetTemp = useCallback(() => setTemp(0),[temp])
________________________________________________________________________________________________________________________
import React, { useCallback, useState } from 'react'
import ReactDOM from 'react-dom'

export const App = () => {
const [temp, setTemp] = useState(100)
const [seconds, setSeconds] = useState(0)

    const resetTemp = useCallback(() => setTemp(0), [])

    const incSec = useCallback(() => setSeconds(seconds + 1), [])

    return <>
        <TempDisplay temp={temp} resetTemp={resetTemp}/>
        <SecDisplay seconds={seconds} incSec={incSec}/>
    </>
}
const TempDisplay = React.memo((props: any) => {
console.log('Render TempDisplay')
return (
<div style={{marginBottom: '10px'}} onClick={props.reset}>
<p>
<b>Температура: </b>{props.temp} &#176;
</p>
<button onClick={props.resetTemp}>Сбросить температуру к 0</button>
</div>
)
})

const SecDisplay = React.memo((props: any) => {
console.log('Render SecDisplay')
return (
<div>
<p><b>Секунды:</b> {props.seconds} c </p>
<button style={{marginRight: '20px'}}
onClick={props.incSec}>
Увеличить время на 1 секунду
</button>
</div>
)
})

ReactDOM.render(<App/>, document.getElementById('root'))

// Почему не корректно работает счетчик времени при нажатии на кнопку (срабатывает только 1 раз) ?
// Найдите в чем причина.
// Исправленную версию строки напишите в качестве ответа

// Пример ответа: const incSec = () => setSeconds(seconds + 1)

    const incSec = useCallback(() => setSeconds(seconds + 1), [seconds])
________________________________________________________________________________________________________________________
import React, { useState } from 'react'
import ReactDOM from 'react-dom'

export const App = () => {
const [temp, setTemp] = useState(10)
const [seconds, setSeconds] = useState(100)

const increaseSeconds = () => setSeconds(seconds + 10)
const increaseTemp = XXX

return <>
<TempDisplay temp={temp} increaseTemp={increaseTemp}/>

       <div>
           <b>Секунды :</b> {seconds} с
           <button style={{marginLeft: '15px'}}
                   onClick={increaseSeconds}>
               Увеличить на 10 секунд
           </button>
       </div>
</>
}
const TempDisplay = React.memo((props: any) => {
console.log('Render TempDisplay')
return (
<div style={{marginBottom: '15px'}}
onClick={props.reset}>
<b>Температура:</b> {props.temp} &#176;
<button style={{marginLeft: '15px'}}
onClick={props.increaseTemp}>
Увеличить температуру на 1 градус
</button>
</div>
)
})

ReactDOM.render(<App/>, document.getElementById('root'));

// Что надо написать вместо XXX для того, чтобы обязательно выполнялись 2 условия:
// 1) При нажатии на кнопку "Увеличить температуру на 1 градус" температура увеличивалась
// 2) Компонент TempDisplay не должен перерисовываться при нажатии на кнопку "Увеличить на 10 секунд"

// Пример ответа: useEffect(() => setCounter(count + 1), [count])

useCallback(() => setTemp(temp + 1), [temp])
________________________________________________________________________________________________________________________
import React, { useState } from 'react'
import ReactDOM from 'react-dom'

type ButtonType = {
id: number
title: string
forAdminOnly: boolean
}
const buttons: ButtonType[] = [
{id: 1, title: 'delete', forAdminOnly: true},
{id: 2, title: 'update', forAdminOnly: true},
{id: 3, title: 'create', forAdminOnly: false},
]

export const App = ({isAdmin}: { isAdmin: boolean }) => {

const [seconds, setSeconds] = useState(0)

const increaseSeconds = () => setSeconds(seconds + 10)

const correctButtons = XXX(() => {
return buttons.filter(b => isAdmin ? true : !b.forAdminOnly)
}, [YYY])

return <>
<ButtonsPanel buttons={correctButtons}/>
<div>
<p>
<b>Секунды: {seconds}</b>
</p>
<button onClick={increaseSeconds}>
Увеличить на 10 секунд
</button>
</div>
</>
}

const ButtonsPanel = React.memo((props: { buttons: Array<ButtonType> }) => {
console.log('Render ButtonsPanel')
return (
<div style={{marginBottom: '15px'}}>
<div style={{marginBottom: '15px'}}>
<b>Панель с кнопками</b>
</div>
<div>
{props.buttons.map(b => <button key={b.id}>{b.title}</button>)}
</div>
</div>
)
})

ReactDOM.render(<App isAdmin={true}/>, document.getElementById('root'))

// Что нужно написать вместо XXX и YYY,
// чтобы избавиться от лишнего перерендера компонента ButtonsPanel
// при нажатии на кнопку "Увеличить на 10 секунд" ?

// Ответ дайте через пробел: 111 222

useMemo buttons - не верно
useMemo isAdmin - предполагаю что верно
_____________________________________________Wednesday_4________________________________________________________________
import {combineReducers, createStore} from 'redux'

let initialState = {items: [{name: 'Dimych'}, {name: 'Ignat'}]}
const usersReducer = (state = initialState, action: any) => {
return state
}

let authInitialState = {login: 'Margo', settings: {theme: 'dark'}}
const authReducer = (state = authInitialState, action: any) => {
return state
}

const store = createStore(combineReducers({
users: usersReducer,
XXX
}))

store.subscribe(() => {
const login = store.getState().auth.login
console.log(login)
})

store.dispatch({type: 'ANY'})
export default store;

// Что нужно написать вместо XXX, чтобы в консоли увидеть 'Margo'?

auth: authReducer
________________________________________________________________________________________________________________________
export const reducer = (state: any, action: any) => {
switch (action.type) {
case 'TRACK-ADDED':
return {
...state,
[action.trackId]: {
id: action.trackId, likesCount: 0
}
}
default:
return state
}
}

const addTrackAC = (trackId: number) => ({type: 'TRACK-ADDED', trackId})

const state = {
12: {id: 12, likesCount: 10},
14: {id: 14, likesCount: 2},
100: {id: 100, likesCount: 0},
}
const newState = reducer(state, xxx)
console.log(newState[300].likesCount === 0)

// Что нужно написать вместо XXX, чтобы в консоли увидеть true?

addTrackAC(300)
________________________________________________________________________________________________________________________
export const reducer = (state: any, action: any) => {
switch (action.type) {
case 'TRACK-DELETED':
return state.filter((track: any) => track.id !== action.trackId)
default:
return state
}
}

const deleteTrackAC =(trackId: number) =>(XXX)


const state = [
{id: 12, likesCount: 10},
{id: 14, likesCount: 2},
{id: 100, likesCount: 0}
]

const newState = reducer(state, deleteTrackAC(14))
console.log(newState.length === 2)

// Что нужно написать вместо XXX, чтобы корректно удалить трек и в консоли увидеть true?

{type: 'TRACK-DELETED', trackId}
________________________________________________________________________________________________________________________
export const reducer = (state: any, action: any) => {
switch (action.type) {
case 'USER-NAME-UPDATED':
return XXX

        default:
            return state
    }
}

const updateUserNameAC = (name: string) => ({type: 'USER-NAME-UPDATED', name})


const state = {
count: 10,
user: {
name: 'Dimych',
age: 18,
isMarried: true,
status: "offline"
},
books: ['you don\'t know JS']
}
const newState = reducer(state, updateUserNameAC('Dmitry'))

console.log(newState.user.name === 'Dmitry')
console.log(newState.books === state.books)
console.log(newState.user !== state.user)

//Что нужно написать вместо XXX, чтобы корректно обновить имя пользователя и в консоли увидеть:  true true true?

{...state, user: {...state.user, name: action.name}}
______________________________________________Thursday_1________________________________________________________________

import axios from 'axios'
import React, { useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client';

// Types
type TodoType = {
id: string;
tile: string;
order: number;
createdAt: string;
updatedAt: string;
complete: boolean;
}


// Api
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const todosAPI = {
getTodos() {
return instance.get<TodoType[]>('todos')
},
}


// App
const App = () => {

const [todos, setTodos] = useState<TodoType[]>([])

useEffect(() => {
todosAPI.getTodos().then((res) => setTodos(res.data))
}, [])

return (
<>
<h2>✅ Список тудулистов</h2>
{
todos.map((t) => {
return (
<div style={t.complete ? {color: 'grey'} : {}} key={t.id}>
<input type="checkbox" checked={t.complete}/>
<b>Описание</b>: {t.tile}
</div>
)
})
}
</>
)
}


const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// При написании типизации по невнимательности было допущено несколько ошибок.
// Напишите через пробел правильные свойства в TodoType, в которых была допущена ошибка.
// Debugger / network / документация вам в помощь

// 🖥 Пример ответа: id status isDone
________________________________________________________________________________________________________________________
import axios from 'axios'
import React, { useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client';

// Types
type PostType = {
id: string
body: string
title: string
userId: string
}


// Api
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const postsAPI = {
getPosts() {
// Promise.resolve() стоит в качестве заглушки, чтобы TS не ругался и код компилировался
// Promise.resolve() нужно удалить и написать правильный запрос для получения постов
return Promise.resolve()
},
}


// App
export const App = () => {

const [posts, setPosts] = useState<PostType[]>([])

useEffect(() => {
postsAPI.getPosts()
.then((res: any) => {
setPosts(res.data)
})
}, [])


return (
<>
<h1>📜 Список постов</h1>
{
posts.length
? posts.map(p => {
return <div key={p.id}><b>title</b>: {p.title}</div>
})
: <h2>Постов нету 😥</h2>
}
</>
)
}


const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// Напишите запрос на сервер для получения всех постов
// Типизацию возвращаемых данных в ответе указывать необязательно, но можно и указать (в ответах учтены оба варианта).
// Исправленную версию строки напишите в качестве ответа.

// 🖥 Пример ответа: return Promise.resolve()
return instance.get<PostType[]>('posts')
________________________________________________________________________________________________________________________
import axios from 'axios'
import React, { ChangeEvent, useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client';

// Types
type CommentType = {
postId: string
id: string
name: string
email: string
body: string
}

// Api
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const commentsAPI = {
getComments() {
return instance.get<CommentType[]>('comments')
},
createComment() {
const payload = {body: 'Это просто заглушка. Backend сам сгенерирует новый комментарий и вернет его вам'}
// Promise.resolve() стоит в качестве заглушки, чтобы TS не ругался и код компилировался
// Promise.resolve() нужно удалить и написать правильный запрос для создания нового комментария
return Promise.resolve()
}
}


// App
export const App = () => {

const [comments, setComments] = useState<CommentType[]>([])

useEffect(() => {
commentsAPI.getComments()
.then((res) => {
setComments(res.data)
})
}, [])

const createPostHandler = () => {
commentsAPI.createComment()
.then((res: any) => {
const newComment = res.data
setComments([newComment, ...comments,])
})
};

return (
<>
<h1>📝 Список комментариев</h1>
<div style={{marginBottom: '15px'}}>
<button style={{marginLeft: '15px'}}
onClick={() => createPostHandler()}>
Добавить новый комментарий
</button>
</div>

      {
        comments.map(c => {
          return <div key={c.id}><b>Comment</b>: {c.body} </div>
        })
      }
    </>
)
}

const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// Напишите запрос на сервер для создания нового комментария.
// Типизацию возвращаемых данных в ответе указывать необязательно, но можно и указать (в ответах учтены оба варианта).
// Исправленную версию строки напишите в качестве ответа.
//
// 🖥 Пример ответа: return Promise.resolve(payload)

return instance.post<CommentType[]>('comments', payload)  -
________________________________________________________________________________________________________________________
import axios from 'axios'
import React, { useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client';

// Types
type PostType = {
body: string
id: string
title: string
userId: string
}


// Api
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const postsAPI = {
getPosts() {
return instance.get<PostType[]>('posts')
},
deletePost(id: string) {
return axios.delete<{ message: string }>(`posts/${id}`)
}
}


// App
export const App = () => {

const [posts, setPosts] = useState<PostType[]>([])

useEffect(() => {
postsAPI.getPosts()
.then((res) => {
setPosts(res.data)
})
}, [])

const deletePostHandler = (id: string) => {
postsAPI.deletePost(id)
.then((res) => {
const newPostsArr = posts.filter(p => p.id !== id)
setPosts(newPostsArr)
})
};

return (
<>
<h1>📜 Список постов</h1>
{posts.map(p => {
return (
<div key={p.id}>
<b>title</b>: {p.title}
<button style={{marginLeft: '15px'}}
onClick={() => deletePostHandler(p.id)}>
x
</button>
</div>
)
})}
</>
)
}


const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// Почему не удаляется post при нажатии на кнопку удаления (х) ?
// Найдите ошибку и вставьте исправленную строку кода в качестве ответа
//
// 🖥 Пример ответа: return axios.delete

return instance.delete<{ message: string }>(`posts/${id}`)
________________________________________________________________________________________________________________________
import axios from 'axios'
import React, { useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client';

// Types
type PhotoType = {
albumId: string
id: string
title: string
url: string
}

type PayloadType = {
title: string
url?: string
}

// Api
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const photoId = '637df6dc99fdc52af974a517'

const photosAPI = {
getPhoto() {
return instance.get<PhotoType>(`photos/${photoId}`)
},
updatePhoto(payload: PayloadType) {
return instance.put<PhotoType>(`photos/${photoId}`, {payload})
}
}


// App
export const App = () => {

const [photo, setPhoto] = useState<PhotoType | null>(null)

useEffect(() => {
photosAPI.getPhoto()
.then((res) => {
setPhoto(res.data)
})
}, [])

const updatePhotoHandler = () => {
// ❗ title и url указаны в качестве заглушки. Server сам сгенерирует новый title
const payload = {
title: 'Новый title',
url: 'data:image/png;base64,iVBORw0FAKEADDRESSnwMZAABJRUrkJggg=='
}
photosAPI.updatePhoto(payload)
.then((res) => {
setPhoto(res.data)
})
};

return (
<>
<h1>📸 Фото</h1>
<div>
<div style={{marginBottom: '15px'}}>
<h1>title: {photo?.title}</h1>
<div><img src={photo?.url} alt=""/></div>
</div>
<button style={{marginLeft: '15px'}}
onClick={updatePhotoHandler}>
Изменить title
</button>
</div>
</>
)
}


const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// При нажатии на кнопку "Изменить title" title должен обновиться,
// но из-за невнимательности была допущена ошибка и изменение не происходит
//
// Найдите и исправьте ошибку
// Исправленную версию строки напишите в качестве ответа.

// 🖥 Пример ответа: photosAPI.updatePhotoTitle(id, title)

return instance.put<PhotoType>(`photos/${photoId}`, payload)
________________________________________________________________________________________________________________________
import axios from 'axios'
import React, { useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client'

type UserType = {
id: string;
name: string;
age: number;
}

// API
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const api = {
getUsers(pageNumber: number) {
return instance.get(`users?pageSize=${3}&pageNumber${pageNumber}`)
},
}

// App
const buttons = [
{id: 1, title: '1'},
{id: 2, title: '2'},
{id: 3, title: '3'},
]

export const App = () => {

const [users, setUsers] = useState<UserType[]>([])
const [currentPage, setCurrentPage] = useState(1)

useEffect(() => {
api.getUsers(currentPage)
.then((res: any) => {
setUsers(res.data.items)
})
}, [currentPage])

const setPageHandler = (page: number) => {
setCurrentPage(page)
};

return (
<>
<h1>👪 Список пользователей</h1>
{
users.map(u => {
return <div style={{marginBottom: '25px'}} key={u.id}>
<p><b>name</b>: {u.name}</p>
<p><b>age</b>: {u.age}</p>
</div>
})
}

      {
        buttons.map(b => {
          return (
            <button key={b.id}
                    style={b.id === currentPage ? {backgroundColor: 'lightblue'} : {}}
                    onClick={() => setPageHandler(b.id)}>
              {b.title}
            </button>
          )
        })
      }
    </>
)
}


const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// При переходе по страницам должны подгружаться новые пользователи.
// Однако в коде допущена ошибка и всегда подгружаются одни и теже пользователи.
// Задача: найти эту ошибку, и исправленную версию строки написать в качестве ответа.

// 🖥 Пример ответа: const [currentPage, setCurrentPage] = useState(page)

=

return instance.get(`users?pageSize=${3}&pageNumber=${pageNumber}`)  
________________________________________________________________________________________________________________________
import axios from 'axios'
import React, { useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client';

// Types
type TodoType = {
id: string;
title: string;
order: number;
createdAt: string;
updatedAt: string;
completed: boolean;
}


// Api
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const todosAPI = {
getTodo(todoId: string) {
return instance.get<TodoType>(`todos/ ${todoId}`)
}
}


// App
export const App = () => {

const [todo, setTodo] = useState<TodoType | null>(null)
const [error, setError] = useState<string>('')

useEffect(() => {
const todoId = "637cb9342f24ad82bcb07d8d"
todosAPI.getTodo(todoId)
.then((res: any) => setTodo(res.data))
.catch(e => {
setError('Ошибка 😰. Анализируй network 😉')
})
}, [])


return (
<>
<h2>✅ Тудулист</h2>
{
!!todo
? <div>
<div style={todo?.completed ? {color: 'grey'} : {}} key={todo?.id}>
<input type="checkbox" checked={todo?.completed}/>
<b>Описание</b>: {todo?.title}
</div>
<h2>Так держать. Ты справился 🚀</h2>
</div>
: <h2 style={{ color: 'red' }}>{error}</h2>
}
</>
)
}


const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// Студент по неопытности допустил одну маленькую ошибку, но из-за нее он не может вывести на экран тудулист.
// Найдите ошибку и вставьте исправленную версию строки кода в качестве ответа
// P.S. Эта ошибка из реальной жизни, студенты часто ошибаются подобным образом и не могут понять в чем дело.

// 🖥 Пример ответа:  .then((res: any) => setTodo(res.data.data))
return instance.get<TodoType>(`todos/${todoId}`)
________________________________________________________________________________________________________________________
import axios from 'axios'
import React, { useEffect, useState } from 'react'
import ReactDOM from 'react-dom/client';

// TYPES
type ProductType = {
id: string
title: string
description: string
price: number
}

type FilmType = {
id: number
nameOriginal: string
description: string
ratingImdb: number
}

type ProductsResponseType = {
total: number
messages: string[]
page: number
pageCount: number
data: ProductType[]
}

type FilmsResponseType = {
total: number
messages: string[]
page: number
pageCount: number
data: FilmType[]
}

type CommonResponseType = {
// your code
}

// Api
const instance = axios.create({baseURL: 'https://exams-frontend.kimitsu.it-incubator.ru/api/'})

const api = {
getProducts() {
return instance.get<ProductsResponseType>('products')
},
getFilms() {
return instance.get<FilmsResponseType>('films')
}
}


// App
const App = () => {
return (
<>
<h1>🛒 Products && 🎦 Films</h1>
<div style={{display: 'flex', justifyContent: 'space-evenly'}}>
<Products/>
<Films/>
</div>
</>
)
}

const Products = () => {

const [products, setProducts] = useState<ProductType[]>([])

useEffect(() => {
api.getProducts()
.then((res) => setProducts(res.data.data))
}, [])

return (
<div style={{width: '45%'}}>
<h2>🛒 Products</h2>
<div>
{
products.map(p => {
return (
<div key={p.id}>
<b>{p.title}</b>
<p>{p.description}</p>
<p>💵 {p.price} $</p>
</div>
)
})
}</div>
</div>
)
}

const Films = () => {

const [films, setFilms] = useState<FilmType[]>([])

useEffect(() => {
api.getFilms()
.then((res) => setFilms(res.data.data))
}, [])

return (
<div style={{width: '45%'}}>
<h2>🎦 Films</h2>
<div>
{
films.map(f => {
return (
<div key={f.id}>
<b>{f.nameOriginal}</b>
<p>{f.description}</p>
<p>⭐ {f.ratingImdb} </p>
</div>
)
})
}</div>
</div>
)
}


const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement);
root.render(<App/>)

// 📜 Описание:
// При запуске проекта на экране вы увидите 2 списка: Products и Films.
// С ними все хорошо, но обратите внимание на типизацию ответов с сервера ProductsResponseType и FilmsResponseType.
// Дублирование типов на лицо.
// Ваша задача написать дженериковый тип CommonResponseType и заменить им дублирующие типы.
// Очередность свойств в типах менять запрещено (по причине что нам будет тяжело перебрать все правильные варианты :) )
// Параметр тип назовите буквой T
//
// В качестве ответа нужно скопировать полностью рабочий дженериковый тип CommonResponseType
//
// 🖥 Пример ответа:
// type CommonResponseType = {
//   total: T
//   messages: T[]
//   page: T
//   pageCount: T
//   data: T[]
// }

type CommonResponseType<T> = {
total: number
messages: string[]
page: number
pageCount: number
data: T[]
}
________________________________________________________________________________________________________________________

________________________________________________________________________________________________________________________

________________________________________________________________________________________________________________________

________________________________________________________________________________________________________________________