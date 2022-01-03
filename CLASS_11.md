# שיעור 10 - JavaScript - ארועים

## מה למדנו בשיעור הקודם
- למדנו על פונקציות
- למדנו איך לכתוב פונקציה (שם, משתנים, ותוכן)

## ארועים
כמו בחיים כאשר קורה ארוע אנחנו מגיבים אליו.
כך גם בקוד, כאשר קורה אירוע אנחנו נרצה להגיב ולבצע פעולה מתאימה

### סוגי ארועים
- Click: לחיצה עם העכבר
- Mouse (move, enter, out): העכבר זז, נכנס או יצא מגבול מסויים
- KeyBoard (keyUp, KeyDoun, KeyPress): לחיצה על מקשים במקלדת

## צורת הכתיבה
```
// מציאת כפתור
const button = document.querySelector('button');

// הגדרת פעולה עבור לחיצה על כפתור
const onClick = () => {
  console.log('לחצו עלי !');
};

// הקשבה לארוע
button.addEventListener('click', onClick);
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
const nameButton = document.getElementById('name-button');
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