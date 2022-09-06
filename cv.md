# Evgenij Yakovlev

## Contacts:  
**Location:** Kiev, Ukraine  
**E-mail:** <tglspfdsfgs@gmail.com>  
**Tel:** +380997246411  
**Telegram:** [@pleasantly_surprized](https://t.me/pleasantly_surprized)  
**Github:** <https://github.com/tglspfdsfgs>  
**Codewars:** <https://www.codewars.com/users/tglspfdsfgs>

## About me:  
qwerty

## Skills:
* HTML + CSS (SASS) [adaptive and responsive design]
* JavaScript [basics, DOM & Events, RegExp, etc]
* BEM
* Git, Github
* gulp
* Sublime Text 

## Code example:  
**Desc:** The base converter, which converts positive integers between arbitrary bases / alphabets
```js
function convert(input, source, target) {
  
  const toDecimal = (input, alpha) => Array.from(input).reduce((sum, char) => sum * alpha.length + alpha.indexOf(char), 0);
  
  let dec = toDecimal(input, source);

  const getIndexesByBase = (decNumber, base) => {
    let arr = [];
    let divisible = decNumber, divider = base;
    
    arr.push(divisible % base);

    while (divisible > 1) {
      divisible = Math.floor(divisible / base);
      if (divisible < 1) break;
      
      arr.push(divisible % base);
    }

    return arr.reverse();
  }
  
  let indexes = getIndexesByBase(dec, target.length);
  
  return  indexes.map( (item, index) => target.charAt(item) ).join('');
}
```  
[This kata solution on Codewars](https://www.codewars.com/kata/reviews/526a569ca578d7e6e3000351/groups/62f5532807268a0001769717)

## Education:
* **Collage:** Vasylkiv College of National Aviation University (2011 - 2015)
  + _Program Subgect Area:_ Maintance of automatic control system
  + _Professonal qualification:_ production process automation technician  

* **freeCodeCamp:** Responsive Web Design (Jan 2022 - Feb 2022)
  + _Certification:_ [link](https://www.freecodecamp.org/certification/tglspfdsfgs/responsive-web-design)  

* **HTML Academy:** Professional HTML and CSS Level 1-2 (Feb 2022 - May 2022)

* **RS Schools Course:** JavaScript/Front-end. Stage 2 ( Sep 2022 - now )  

* **Books and resources:** 
  + Head First HTML and CSS: A Learner's Guide to Creating Standards-Based Web Pages
  + JavaScript Manual on javascript.info (learn.javascript.ru)

## Languages: 
* English - B1+
* Russian - Native
* Ukranian - Native
