---
language:
  - he
license: odc-by
pretty_name: נתוני הכנסת הפתוחים — Israel Knesset Open Data
size_categories:
  - 1M<n<10M
tags:
  - parliament
  - israel
  - knesset
  - legislation
  - government
  - democracy
  - hebrew
  - politics
  - open-data
task_categories:
  - text-classification
  - question-answering
  - summarization
---

# 🏛️ נתוני הכנסת הפתוחים — Israel Knesset Open Data

מאגר הנתונים המקיף ביותר של הכנסת — הפרלמנט של מדינת ישראל.

**44 טבלאות | ~1.5 מיליון רשומות | כל הכנסות (1-26)**

<div dir="rtl">

> הדמוקרטיה דורשת שקיפות. שקיפות דורשת נתונים. נתונים דורשים נגישות.

</div>

## 📊 סקירת הנתונים

הנתונים מקורם ב-[OData API הרשמי של הכנסת](https://knesset.gov.il/Odata/ParliamentInfo.svc/) ומכסים את כל הפעילות הפרלמנטרית מכנסת 1 (1949) ועד היום.

### 👥 אנשים ותפקידים

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_Person` | חברי כנסת — פרטים אישיים | 1,184 |
| `KNS_PersonToPosition` | מינויים לתפקידים — שר, יו"ר ועדה וכו' | 23,483 |
| `KNS_Position` | סוגי תפקידים | 29 |
| `KNS_Faction` | סיעות בכל הכנסות | 544 |
| `KNS_MkSiteCode` | קודי אתר לחברי כנסת | 1,111 |

### 🏢 ועדות

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_Committee` | ועדות הכנסת | 2,900 |
| `KNS_CommitteeSession` | ישיבות ועדות | 107,740 |
| `KNS_CmtSessionItem` | נושאים בישיבות ועדות | 78,329 |
| `KNS_JointCommittee` | ועדות משותפות | 1,174 |
| `KNS_CmtSiteCode` | קודי אתר לוועדות | 720 |
| `KNS_BroadcastCommitteSession` | שידורי ישיבות ועדות | 107,752 |
| `KNS_DocumentCommitteeSession` | מסמכי ישיבות ועדות (פרוטוקולים, הזמנות) | 196,085 |

### 📜 חקיקה — הצעות חוק

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_Bill` | הצעות חוק | 59,986 |
| `KNS_BillInitiator` | יוזמי הצעות חוק | 169,510 |
| `KNS_BillHistoryInitiator` | היסטוריית יוזמים | 10,390 |
| `KNS_BillName` | שמות הצעות חוק (כולל שינויים) | 27,812 |
| `KNS_BillSplit` | פיצולי הצעות חוק | 818 |
| `KNS_BillUnion` | איחודי הצעות חוק | 1,563 |
| `KNS_DocumentBill` | מסמכים מצורפים להצעות חוק | 110,492 |

### ⚖️ חקיקה — חוקים

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_IsraelLaw` | חוקי מדינת ישראל | 1,993 |
| `KNS_IsraelLawBinding` | קשרים בין חוקים | 373 |
| `KNS_IsraelLawClassificiation` | סיווגי חוקים | 2,853 |
| `KNS_IsraelLawMinistry` | משרדים אחראים על חוקים | 1,695 |
| `KNS_IsraelLawName` | שמות חוקים (כולל שינויים) | 2,148 |
| `KNS_LawBinding` | הפניות חוקיות מחייבות | 15,046 |
| `KNS_DocumentIsraelLaw` | מסמכי חוקים | 0 |

### 📋 חקיקת משנה

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_SecondaryLaw` | חקיקת משנה (תקנות, צווים) | 59,876 |
| `KNS_SecLawAuthorizingLaw` | חוקים מסמיכים לחקיקת משנה | 67,827 |
| `KNS_SecLawRegulator` | גורמים מתקינים | 4,817 |
| `KNS_SecToSecBinding` | קשרים בין תקנות | 23,763 |
| `KNS_DocumentSecondaryLaw` | מסמכי חקיקת משנה | 6,847 |

### 🎤 מליאה

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_PlenumSession` | ישיבות מליאה | 8,743 |
| `KNS_PlmSessionItem` | נושאים בישיבות מליאה | 167,957 |
| `KNS_PlenumVote` | הצבעות במליאה | 34,916 |
| `KNS_PlenumVoteResult` | תוצאות הצבעות (מאוחד) | 50 |
| `KNS_DocumentPlenumSession` | מסמכי ישיבות מליאה | 74,385 |

### ❓ שאילתות (פניות)

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_Query` | שאילתות חברי כנסת לממשלה | 42,620 |
| `KNS_DocumentQuery` | מסמכי שאילתות | 7,134 |

### 📅 סדר יום

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_Agenda` | נושאי סדר היום | 42,141 |
| `KNS_DocumentAgenda` | מסמכי סדר יום | 27,269 |

### 🔧 טבלאות עזר

| טבלה | תיאור | רשומות |
|-------|--------|---------|
| `KNS_Status` | קודי סטטוס | 82 |
| `KNS_ItemType` | סוגי פריטים | 8 |
| `KNS_GovMinistry` | משרדי ממשלה | 922 |
| `KNS_KnessetDates` | תקופות כנסת ומושבים | 164 |

## 📁 מבנה הקבצים

```
data/
├── KNS_Person/
│   ├── manifest.yaml          # סכמה, מקור, checksum
│   └── KNS_Person_0.jsonl     # נתונים
├── KNS_Bill/
│   ├── manifest.yaml
│   ├── KNS_Bill_0.jsonl       # 0-49999
│   └── KNS_Bill_1.jsonl       # 50000+
├── ...
└── (44 טבלאות)
manifest.yaml                   # מניפסט ראשי עם סיכום כולל
```

כל קובץ JSONL מכיל עד 50,000 רשומות. קבצים גדולים מפוצלים אוטומטית.

## 🔍 מניפסטים

כל טבלה כוללת `manifest.yaml` עם:
- **סכמה מלאה** — שמות שדות, טיפוסים, nullable
- **מקור** — כתובת API, תאריך חילוץ
- **checksums** — SHA-256 לכל קובץ
- **id_range** — טווח מזהים (min/max) לגישה מהירה
- **פרובננס** — W3C PROV + Dublin Core

## 🚀 שימוש

### Python
```python
from datasets import load_dataset

# טעינת טבלה בודדת
bills = load_dataset("ZeAlenu/knesset-data", data_files="data/KNS_Bill/*.jsonl")

# טעינת כל הנתונים
all_data = load_dataset("ZeAlenu/knesset-data")
```

### CLI
```bash
# הורדה מלאה
git clone https://huggingface.co/datasets/ZeAlenu/knesset-data

# הורדה חלקית (טבלה ספציפית)
git clone --no-checkout https://huggingface.co/datasets/ZeAlenu/knesset-data
cd knesset-data
git sparse-checkout set "data/KNS_Bill"
git checkout main
```

## 🔄 עדכונים

הנתונים מסונכרנים מה-API הרשמי של הכנסת. כל שינוי מתועד ב-commit history.

**Mirror:** הנתונים זמינים גם ב-[GitHub](https://github.com/ZeAlenu/knesset-data).

## 📜 רישיון

הנתונים מקורם ב-[אתר הכנסת הפתוח](https://main.knesset.gov.il/Activity/Info/Pages/Databases.aspx) — מידע ציבורי של מדינת ישראל.

רישיון: [Open Data Commons Attribution License (ODC-BY)](https://opendatacommons.org/licenses/by/).

## 🏗️ מי אנחנו

**[זה עלינו (ZeAlenu)](https://zan.org.il)** — תנועה אזרחית ציונית לשקיפות, חירויות אזרח וחינוך ריבוני.

אנו מאמינים שנתונים פתוחים הם תנאי הכרחי לדמוקרטיה בריאה. פרויקט זה נועד להנגיש את המידע הפרלמנטרי לכל אזרח, חוקר ומפתח.

---

<div dir="rtl" align="center">

**🇮🇱 נתוני העם, לעם, למען העם**

</div>
