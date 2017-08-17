הרגלי עבודה נכונים בעולם הסייבר
====

שם מפוצץ להרצאה Mind Blowing.
----

---


מבוא
====

## אז מה בעצם נלמד בהדרכה זו?
- איך אנחנו מארגנים את הפרויקטים שלנו בצורה נכונה יותר?
- דווקא בגף שתחלופת כוח האדם גבוהה, איך להקל על מעבר של פרויקטים בין אנשים?
- איך אנחנו יכולים לכתוב תכניות בשפת C וב-LabView שיהיו יותר קלות לקריאה, ויותר קלות לשילובן בתכניות אחרות?

---

נושאי ההרצאה
===

- [Git](#git)
- [שמות קבצים ותיקיות](#file-names)
- [הרגלי כתיבה וארגון של תכנה](#writing-habits)

---

# חלק 1: Git {#git}

TODO

---

# חלק 2: ארגון הקבצים בשרת ובמחשבים האישיים {#file-names}

## מדוע זה חשוב לבחור שמות נכונים לקבצים שלנו?

- יזכרו אתכם לטובה (לומברוזו)
- יוכלו להשתמש בידע שצברתם ובעבודה שעשיתם

בחלק זה של ההדרכה, נלמד את הנושאים הבאים:

- איך החברות הגדולות מנהלות את הפרויקטים שלהם והקבצים שלהם?
- איך אפשר ללמוד על הגישות הללו רק ממתן תשומת לב אפילו רק מגלישה שגרתית באינטרנט?
- מה הדגשים לפיהם הכי נכון לתת שמות הנותנים לקבצים ולתיקיות?

---

## מה עושים בחברות הגדולות?

### דוגמאות

בחלק זה של השיעור, נלמד על הרגלים שהקנו לעצמן חברות ותאגידים גדולים בבחירה ובניהול נכון של קבצים ותיקיות.

נעשה זאת בעיקר דרך מבט על שורת ה-URL בדפדפן המרשתת בכל עמוד של אתר מאת האתרים של החברות הללו.

---

<H4 dir=ltr>[Github.com](https://github.com) & [Gitlab.com](https://gitlab.com)</H4>

- כל פרויקט (repository) נמצא תחת המסלול:

<div dir=ltr>
`https://git{hub,lab}.com/<owner>/<project>`
</div>

- למשתמשים יש אפשרות ליצור ארגון תחתיו הם יכולים לשייך את עצמם ועוד משתמשים מבלי שהשם שלהם או של מישהו אחר יהיה דווקא זה שלוקח את כל הקרדיט. דוגמה:

<div dir=ltr>
[`https://gitlab.com/gaf1/bamba`](https://gitlab.com/gaf1/bamba)
</div>

- חוץ מהשמות של כל פרויקט, יש אחידות בדפי האינטרנט תחת כל פרויקט. לדוגמה, באגים תמיד ימצאו בכתובת הזו:

<div dir=ltr>
[`https://gitlab.com/gaf1/sachnat/issues`](https://gitlab.com/gaf1/sachnat/issues)
</div>

- ואם נרצה להגיע לבאג ספציפי, לכל באג יש מספר:

<div dir=ltr>
[`https://gitlab.com/gaf1/sachnat/issues/350`](https://gitlab.com/gaf1/sachnat/issues/350)
</div>

- 'מזלוגים' (Forks).

<div dir=ltr>
[`https://gitlab.com/bamtza108/sachnat`](https://gitlab.com/bamtza108/sachnat)
</div>

---

<H4 dir=ltr>[npmjs.com](https://npmjs.com)</H4>

- לכל חבילת JavaScript יש שם ייחודי וכולן למעשה נמצאות באותה תיקייה:

<div dir=ltr>
`https://npmjs.com/package/<package-name>`
</div>

לדוגמה:

<div dir=ltr>
[`https://npmjs.com/package/express`](https://npmjs.com/package/express)
</div>

---

<H4 dir=ltr>[twitter.com](https://twitter.com)</H4>

- לכל משתמש יש שם ייחודי, לדוגמה:

<div dir=ltr>
[`https://twitter.com/tpope`](https://twitter.com/tpope)

> Vim plugin Artist
</div>

- כל משתמש כותב סטטוס והלינק לסטטוס יהיה בלינק כגון:

<div dir=ltr>
[`https://twitter.com/sailorhg/status/484501845209919488`](https://twitter.com/sailorhg/status/484501845209919488)

> I care a lot about making my git history look nice. One might call me cherry-picky.
</div>

---

<H4 dir=ltr>[reddit.com](https://reddit.com)</H4>

- לכל אשכול (subreddit), יש שם ייחודי, לדוגמה:

<div dir=ltr>
[`https://reddit.com/r/linux`](https://reddit.com/r/linux)
</div>

- בכל אשכול, כל post יימצא תחת הכתובת:

<div dir=ltr>
[`https://reddit.com/r/linux/comments/6tysw2/when_your_cat_likes_to_stand_on_warm_things_that/`](https://reddit.com/r/linux/comments/6tysw2/when_your_cat_likes_to_stand_on_warm_things_that/)
</div>

- כל post מקבל מקבל קוד רנדומלי כמו ב-twitter אבל ב-reddit יש קשר חזק בין תוכנו של ה-post לכתובת ה-URL שלו.

---

### סיכום

- השמות של כל משתמש, פרויקט, תיקייה, קובץ (או עמוד אינטרנט) הם קצרים, ברורים וייחודיים.
- כל חברה/אתר מגדיר הגבלות שונות לבחירת שמות, מה שמשתוף לכולם זה ש**אין להם רווחים**, לא למשתמשים, לפרויקטים לתיקיות ולקבצים..

---

## דוגמאות ליתרונות בקביעת כללים כאלו

### ניהול חבילות JavaScript בסביבת עבודה עם NPM

- לכל חבילת JavaScript יש תלות בחבילות אחרות.
- כל חבילת JavaScript מציינת בקובץ שנקרא `package.json` את רשימת החבילות שבהן היא תלויה, בנוסף לעוד מידע על החבילה (רישיון, תיאור כללי, גרסה..).
- הקובץ `package.json` כתוב בפורמט `json` שנועד לקריאה בקלות ע"י JavaScript.
- כל אחד יכול לכתוב קובץ `pcakage.json` - הוא נוח לקריאה גם של בני-אדם וגם מכונות.
- כשמישהו מחליט לכתוב חבילת JavaScript או יישומון מרשתת, הוא יכול לכתוב את הקובץ `package.json` לחבילה שלו, ובו את הרשימה של כל החבילות בהן הוא תלוי.
- פקודת `npm install` מתקינה אוטומטית את כל החבילות לפי תוכנו של `package.json`.
- כל החבילות מותקנות בתיקיית `node_modules` - כך זה בכל חבילת JavaScript.

---

כך נראה קובץ `package.json` של חבילת JavaScript לדוגמה:
```json

```

---

כך נראה תהליך ההתקנה של החבילות בהן יש תלות:

<div align=center>
![Example of node modules installations]()
</div>

---

כך נראית תיקיית `node_modules` בחבילת לדוגמה (`request`):

<div align=center>
![Example of node_modules directory]()
</div>

---

### סטנדרטים בכתיבת תכנות וחבילות Python

- גם ל-`Python` יש את `Pypi`.
- כל חבילה כזו, חייבת להגיע עם הקובץ `setup.py` בו מצוינות החבילות בהן היא תלויה בנוסף לעוד מידע על החבילה (רישיון, תיאור כללי, גרסה..).

דוגמה לקובץ `setup.py` של חבילת `khal`:

```python

```

---
## דוגמאות לחסרונות של אי קביעת כללים כאלו


