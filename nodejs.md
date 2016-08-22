# Node JS

## Internationalizaion i18n

### Intl
 

>Collator: Sorts things in order

### Date
- Date().ToString() - don't use
- Date().toLocaleString()

### Number
- Number().toString() - don't use
- Number().toLocaleString()

### String
```javascript
- "a" < "b" - don't use
- "u" === "U" - doesn't work either
- 'I'.toLowerCase() === 'i'.toLowerCase() - does not work for some languages
- "abc".localeCompare("abc")
- ('u' + <unifier>).normalize("NFC")
- 'I'.toLocaleLowerCase('tr') == 'i'.toLocaleLowerCase('tr')
```
