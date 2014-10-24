Mobile Web Dev Tips
===================

Micro tips for mobile web dev.


#iOS
###JavaScript
*   для блокирования браузерного скрола без блокировки стандартного  поведения ссылок необходимо сделать `e.preventDefault();` в первом `touchmove`

###CSS

#Android
##Chrome for Android
###JavaScript
*   для блокирования браузерного скрола без блокировки стандартного  поведения ссылок необходимо сделать `e.preventDefault();` **в каждом** `touchmove`

###CSS

##Android Browser
###JavaScript
*   для блокирования браузерного скрола без блокировки стандартного  поведения ссылок необходимо сделать `e.preventDefault();` **в каждом** `touchmove`

###CSS

##Android FireFox
###JavaScript
###CSS

##Common
###JavaScript
*   проверка наличия нативного скролла

```javascript
function detect (testElement) {
    var computedStyle = documentDefaultView.getComputedStyle(testElement, null);
    return (computedStyle.webkitOverflowScrolling === 'touch')
        && ((computedStyle.overflowX === 'auto')
        || (computedStyle.overflowX === 'scroll')
        || (computedStyle.overflowY === 'scroll'));
}
```
