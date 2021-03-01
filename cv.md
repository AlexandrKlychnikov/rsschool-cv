# ALEKSANDR KLYCHNIKOV

**Contacts**

* +7 911 345 66 10
* [klychnikov75@mail.ru](mailto:klychnikov75@mail.ru)
* [GitHub](https://github.com/AlexandrKlychnikov)

## About me

I am a bank officer. I have a lot of experience working in the credit departments of various banks.
I've always been interested in programming. In my professional career, 
I have repeatedly beaten routine tasks with the help of VBA.
I recently decided to retrain as a front-end developer. 
Responsible, attentive to details, quick learner-that's all about me.

## Training

1. [HTML Academy](https://htmlacademy.ru/)
2. [Learn JS](https://learn.javascript.ru/)
3. [Codewars](https://www.codewars.com/)

## Skills

* HTML/CSS & Pug/Sass
* JavaScript
* Git
* Webpack, npm

## `Code examples`   

``` javascript
//accum("RqaEzty") -> "R-Qq-Aaa-Eeee-Zzzzz-Tttttt-Yyyyyyy"

function accum(str) {
  let newS = str.split('').reduce((acc, cur, i) => {
    let letter = ''
    for (let n=1; n <= i+1; n++) {
      letter += cur; 
    } 
    let newLetter = letter[0].toUpperCase() + letter.toLowerCase().slice(1)
    acc.push(newLetter);
    return acc;
  }, [])
  return newS.join('-');
}

//refactoring

function accum(str) {
  return str.split('').map((c, i) => (c.toUpperCase() + c.toLowerCase().repeat(i))).join('-');
}
```

