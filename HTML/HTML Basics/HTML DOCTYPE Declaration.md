### Что такое DOCTYPE в HTML?

DOCTYPE — это декларация, размещаемая в начале HTML-документов. Она сообщает браузеру о типе документа и версии, что помогает обеспечить правильное отображение. DOCTYPE не является HTML-тегом. Наиболее распространённый DOCTYPE — `<!DOCTYPE html>`, используемый для HTML5, который соответствует современным веб-стандартам.

### Декларация DOCTYPE

Декларация DOCTYPE размещается в верхней части веб-страницы перед другими элементами и является обязательной по стандартам HTML. Это гарантирует правильное отображение страницы в браузерах и соблюдение указанной версии HTML.

_Примечание: DOCTYPE для HTML5 нечувствителен к регистру._

**Синтаксис DOCTYPE в HTML**
```html
< !DOCTYPE html >
```

### Использование DOCTYPE
- **HTML 4.01**: DOCTYPE ссылается на определение типа документа (DTD), которое определяет структуру и допустимые элементы XML-документа.
- **SGML Basis**: HTML 4.01 основан на Стандартизированном Обобщенном Языке Разметки (SGML), что требует ссылки на DTD в декларации DOCTYPE.
- **Strict DTD**: Используется для веб-страниц, исключающих устаревшие атрибуты и элементы, что способствует применению CSS для оформления.
- **Transitional DTD**: Позволяет использовать устаревшие элементы и атрибуты, упрощая переход от старых версий HTML к более современным практикам.
- **Frameset DTD**: Специально используется для веб-страниц с фреймами, определяя структуру и допустимые элементы для таких макетов.

### Общие декларации DOCTYPE для различных версий HTML и XHTML
- **HTML 5**:
```html
<!DOCTYPE html>
```
- **HTML 4.01 Strict**:
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
    "http://www.w3.org/TR/html4/strict.dtd">
```
- **HTML 4.01 Transitional**:
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
    "http://www.w3.org/TR/html4/loose.dtd">
```
- **HTML 4.01 Frameset**:
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN"
    "http://www.w3.org/TR/html4/frameset.dtd">
```
- **XHTML 1.0 Strict**:
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" 
    "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```
- **XHTML 1.0 Transitional**:
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" 
    "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```
- **XHTML 1.0 Frameset**:
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" 
    "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">
```
- **XHTML 1.1**:
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" 
    "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
```