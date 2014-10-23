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
    var completedStyle = documentDefaultView.getComputedStyle(testElement, null);
    return (completedStyle.webkitOverflowScrolling === 'touch')
        && ((completedStyle.overflowX === 'auto')
        || (completedStyle.overflowX === 'scroll')
        || (completedStyle.overflowY === 'scroll'));
}
```
