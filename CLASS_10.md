# שיעור 10 - JavaScript - פונקציות

## מה למדנו בשיעור הקודם
- למדנו על איך להוסיף תנאים לקוד
- `if` & `else`

## פונקציות
פונקציה היא קטע קוד שמרכז בתוכו מספר פקודות, הפונקציה יכולה להחזיר תוצאה שונה על בסיס המשתנים שהיא קיבלה.
לדוגמה תנור, התנור יכול לקבל מגבן רחב של מאפים הוא מבצע פונקייה של אפייה ואנחנו מקבלים מאפה.

## צורת הכתיבה
```
const printMyName = (myName) => {
  console.log(myName);
}

const multiply = (a, b) => {
  return a * b;
}
```


## עשו זאת בעצמכם
1. הוסיפו את רשימת הדפים למשחק שלכם באזור המיועד ל JavaScript
```
const pages = [
  "welcome",
  "category",
  "the-game"
];
```
2. הוסיפו את קטע הקוד הבא
```
nameButton.addEventListener('click', () => {
  name = document.getElementById('name').value;
  setCurrentPage(1);
  document.getElementById('player-name').innerText = name;
});
```
3. הוסיפו את הפונקציה הבאה
```
const setCurrentPage = (page) => {
  document.querySelector(`.${curentPage}`).classList.add('hidden');
  curentPage = pages[page];
  document.querySelector(`.${curentPage}`).classList.remove('hidden');
}
```
4. לחצו על כפתור ה לייק