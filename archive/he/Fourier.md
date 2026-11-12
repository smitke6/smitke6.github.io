---
layout: post
category: joke
title: "התמרות פורייה לא-יעילות"
date: 2017-05-30
---

<div dir="rtl" lang="he" markdown="1">

<div style="display: flex; flex-wrap: wrap; justify-content: space-between;">

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Lazy Fourier Transform (LFT)**<br>
עבור וקטור קלט $ \mathbf{x} $:

1. רפד באפסים עד שגודל $ \mathbf{x} $ יהיה חזקה שלמה של 2
2. רפד באפסים עד שגודל $ \mathbf{x} $ יהיה חזקה שלמה של 3
3. זרוק לו עוד מיליארד אפסים
4. עבור ראשוני אקראי $ p $, רפד באפסים עד שגודל $ \mathbf{x} $ יהיה חזקה שלמה של $ p $
5. זהו, עכשיו בקירוב טוב $ \mathbf{x} \equiv 0 $, והתמרת פורייה של אפס זה אפס, אז תחזיר אפס

</div>

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Slow Fourier Transform (SFT)**<br>
עבור וקטור קלט $ \mathbf{x} $:

1. אתחל $ \mathbf{y}=0 $
2. מצא ל-$ \mathbf{x} $ fit שהוא גאוסיאן
3. התמרת פורייה של גאוסיאן זה גאוסיאן! אני זוכר כי הייתה לי בדיחה על זה באחד הפוסטים הקודמים
4. הוסף ל-$ \mathbf{y} $ את הגאוסיאן המותמר והחסר מ-$ \mathbf{x} $ את הגאוסיאן המקורי
5. חזור על התהליך עד ש-$ \mathbf{x}=0 $, ואז החזר את $ \mathbf{y} $

**סיבוכיות:** לא יודע, זה בכלל מתכנס?

</div>

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Quantum Fourier Transform (QFT)**

1. חכה שיצליחו לבנות מחשב קוונטי אמיתי עם מספר גדול של קיוביטים
2. הרץ עליו את האלגוריתם הידוע ל-QFT, שלוקח רק $ O(\log n) $

אה, רצית את וקטור הפלט בצורה של וקטור רגיל, ולא נוח לך שהרכיבים שלו שמורים כפאזות של קיוביטים? טוב זו לא בעיה, יש שיטה... _\*מלמול\*_ מעגל הערכת-פאזה... _\*מלמול\*_ וזהו, שיהיה בהצלחה!

</div>

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Bogo Fourier Transform (BFT)**<br>
עבור וקטור קלט $ \mathbf{x} $:

1. הגרל וקטור אקראי $ \mathbf{y} $
2. חשב את התמרת פורייה ההפוכה של $ \mathbf{y} $, שנסמנה $ \text{FT}^{-1} [ \mathbf{y} ] $
3. אם $ \mathbf{x} = \text{FT}^{-1} [ \mathbf{y} ] $, החזר $ \mathbf{y} $. אחרת חזור ל-1

**הערה:** איך לחשב את התמרת פורייה ההפוכה בשלב 2? אמממ... יש פונקציה לזה ב-MATLAB, נראה לי הכי טוב.

</div>

</div>

</div>
