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
</script> getElementById
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

________________________________________________________________________________________________________________________



























