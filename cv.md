# Arguchinsky Alexey
### Contacts
* *Phone number* : +375333607138;
* *Email* : arguchinsky55@gmail.com;
* *Facebook* : [facebook-link](https://www.facebook.com/people/%D0%90%D0%BB%D0%B5%D0%BA%D1%81%D0%B5%D0%B9-%D0%90%D1%80%D0%B3%D1%83%D1%87%D0%B8%D0%BD%D1%81%D0%BA%D0%B8%D0%B9/100001835178675);
* *GitHub* : [github-link](https://github.com/arguchinsky);
* *Telegram* : [telegram-link](https://t.me/arguchinsky);
* *LinkedIn* : [linkedin-link](https://www.linkedin.com/in/%D0%B0%D0%BB%D0%B5%D0%BA%D1%81%D0%B5%D0%B9-%D0%B0%D1%80%D0%B3%D1%83%D1%87%D0%B8%D0%BD%D1%81%D0%BA%D0%B8%D0%B9-11193b18a/);

## About me
I am a developer (embedded software). I work for an enterprise **"Электроприбор"**. I started my carrier in the 2010 year.

I am developing embedded software for the devices used in the energy sector(converters, ammeters, voltmeters, wattmeters, etc.). At this moment, I work on implementing the Protocol **"IEC101"** in the devices manufacturing our enterprise. I'm also adding new functionality for some modifications to our devices.
Also, I am engaged in administrating our [website](https://www.electropribor.by/).

Now I want to change my specialization from the Embedded to the Front-end development.

I'm studying **Front-end** development on resources:
* **[MDN](https://developer.mozilla.org/ru/)**
* **[LearnJavaScript](https://learn.javascript.ru/)**
* **[Metanit](https://metanit.com/)**
* **[React](https://ru.reactjs.org/)**
* **[Codeacademy](https://www.codecademy.com)**

### Skills
* ***C++***
* ***HTML***
* ***CSS***
* ***SCSS/SASS***
* ***Javascript***
* ***React***
* ***Redux***
* ***Git***
* ***Webpack***
* ***Eslint***
* ***Babel***
### Code examples:
* ***Javascript:***

```javascript
"use strict";
const gallery = document.querySelector('.gallery');
const nextBtn = document.querySelector('.next');
const prevBtn = document.querySelector('.prev');

const width = 960;

const leftPos = gallery.getBoundingClientRect().left;
const endSwitch = (gallery.getBoundingClientRect().width * -1) + width ;

let position = 0;

const prevSlide = () => {
    if (position < 0) position += width;
    else position = 0;
    gallery.style.marginLeft = position+'px';
    console.log(position);
}

const nextSlide = () => {
    if (position > endSwitch )position -= width;
    else position = endSwitch;
    gallery.style.marginLeft = position+'px';
    console.log(position);
}

nextBtn.addEventListener('click', nextSlide);
prevBtn.addEventListener('click', prevSlide); 
```

* ***JSX:***

```jsx
import React from 'react';
import PropTypes from 'prop-types';
import Color from '../color/color.jsx';

const ColorList = ({colors, onRemove, onRate}) =>
    <div className="color-list">
        {
            (colors.length === 0) ?
                <p>No Colors Listed. (Add a Color)</p> :
                colors.map(color => <Color key={color.id} {...color}
                                            onRate={(rating) => onRate(color.id, rating)}
                                            onRemove={() => onRemove(color.id)}/>)
        }
    </div>

ColorList.propTypes = {
    colors: PropTypes.array,
    onRemove: PropTypes.func,
    onRate: PropTypes.func,
}

ColorList.defaultProps = {
    colors: [],
    onRemove: ()=>{},
    onRate: ()=>{},
}

export default ColorList;
```

### My project
*[Weather app](https://arguchinsky-weather.surge.sh/)*.

### Experience
* **[Codeacademy](https://www.codecademy.com/profiles/arguchinsky-alexey)**
* **[Codewars](https://www.codewars.com/users/arguchinsky)**

### Education
In the 2009 year, I am finished Vitebsk State University named after P.M.Masherov. I have a Bachelor's degree in physics and informatics.

### English
I don't know my English level.
I read the technical documentation.
But I have some difficulty in conversations.
I understand my interviewer if he doesn't speak quickly.
I don't have much experience communicating with other people in English.
