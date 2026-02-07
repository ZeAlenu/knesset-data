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
---

<div dir="rtl">

# 🇮🇱 נתוני הכנסת הפתוחה

מאגר נתונים פתוח של הכנסת — ישירות מה-API הרשמי, בפורמט JSONL מחולק לקבצים.

**מקור:** [OData API של הכנסת](https://knesset.gov.il/OdataV4/ParliamentInfo)
**רישיון:** CC-BY-SA-4.0
**תחזוקה:** [זה עלינו](https://zan.org.il)

כל קובץ JSONL מכיל שורה אחת לכל רשומה, ממוין לפי `Id`.

</div>

---

# 🇮🇱 Knesset Open Data

Open dataset of the Israeli Knesset (parliament) — sourced directly from the official API, stored as partitioned JSONL files.

**Source:** [Knesset OData API](https://knesset.gov.il/OdataV4/ParliamentInfo)
**License:** CC-BY-SA-4.0
**Maintained by:** [ZeAlenu](https://zan.org.il)

## 📊 Tables (44 total, ~1.5M records)

### 👥 אנשים ותפקידים — People & Positions

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_Person` | חברי כנסת — MK personal details | 1,184 |
| `KNS_PersonToPosition` | מינויים לתפקידים — Position appointments | 23,483 |
| `KNS_Position` | סוגי תפקידים — Position types | 29 |
| `KNS_Faction` | סיעות — Factions | 544 |
| `KNS_MkSiteCode` | קודי אתר לח"כים — MK site codes | 1,111 |

### 🏢 ועדות — Committees

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_Committee` | ועדות הכנסת — Committees | 2,900 |
| `KNS_CommitteeSession` | ישיבות ועדות — Committee sessions | 107,740 |
| `KNS_CmtSessionItem` | נושאים בישיבות — Session agenda items | 78,329 |
| `KNS_JointCommittee` | ועדות משותפות — Joint committees | 1,174 |
| `KNS_CmtSiteCode` | קודי אתר — Committee site codes | 720 |
| `KNS_BroadcastCommitteSession` | שידורי ישיבות — Session broadcasts | 107,752 |
| `KNS_DocumentCommitteeSession` | מסמכי ועדות — Committee documents | 196,085 |

### 📜 הצעות חוק — Bills

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_Bill` | הצעות חוק — Bills | 59,986 |
| `KNS_BillInitiator` | יוזמי הצעות חוק — Bill initiators | 169,510 |
| `KNS_BillHistoryInitiator` | היסטוריית יוזמים — Initiator history | 10,390 |
| `KNS_BillName` | שמות הצעות חוק — Bill names | 27,812 |
| `KNS_BillSplit` | פיצולי הצעות — Bill splits | 818 |
| `KNS_BillUnion` | איחודי הצעות — Bill unions | 1,563 |
| `KNS_DocumentBill` | מסמכי הצעות חוק — Bill documents | 110,492 |

### ⚖️ חוקים — Laws

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_IsraelLaw` | חוקי מדינת ישראל — Israeli laws | 1,993 |
| `KNS_IsraelLawBinding` | קשרים בין חוקים — Law bindings | 373 |
| `KNS_IsraelLawClassificiation` | סיווגי חוקים — Law classifications | 2,853 |
| `KNS_IsraelLawMinistry` | משרדים אחראים — Responsible ministries | 1,695 |
| `KNS_IsraelLawName` | שמות חוקים — Law names | 2,148 |
| `KNS_LawBinding` | הפניות חוקיות — Legal references | 15,046 |
| `KNS_DocumentIsraelLaw` | מסמכי חוקים — Law documents | 0 |

### 📋 חקיקת משנה — Secondary Legislation

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_SecondaryLaw` | תקנות וצווים — Regulations & orders | 59,876 |
| `KNS_SecLawAuthorizingLaw` | חוקים מסמיכים — Authorizing laws | 67,827 |
| `KNS_SecLawRegulator` | גורמים מתקינים — Regulators | 4,817 |
| `KNS_SecToSecBinding` | קשרים בין תקנות — Regulation bindings | 23,763 |
| `KNS_DocumentSecondaryLaw` | מסמכי חקיקת משנה — Secondary law docs | 6,847 |

### 🎤 מליאה — Plenum

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_PlenumSession` | ישיבות מליאה — Plenum sessions | 8,743 |
| `KNS_PlmSessionItem` | נושאים בישיבות — Plenum agenda items | 167,957 |
| `KNS_PlenumVote` | הצבעות — Votes | 34,916 |
| `KNS_PlenumVoteResult` | תוצאות הצבעות — Vote results | 50 |
| `KNS_DocumentPlenumSession` | מסמכי מליאה — Plenum documents | 74,385 |

### ❓ שאילתות — Queries

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_Query` | שאילתות לממשלה — Parliamentary queries | 42,620 |
| `KNS_DocumentQuery` | מסמכי שאילתות — Query documents | 7,134 |

### 📅 סדר יום — Agenda

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_Agenda` | נושאי סדר היום — Agenda items | 42,141 |
| `KNS_DocumentAgenda` | מסמכי סדר יום — Agenda documents | 27,269 |

### 🔧 טבלאות עזר — Reference Tables

| Table | Description | Records |
|-------|-------------|---------|
| `KNS_Status` | קודי סטטוס — Status codes | 82 |
| `KNS_ItemType` | סוגי פריטים — Item types | 8 |
| `KNS_GovMinistry` | משרדי ממשלה — Government ministries | 922 |
| `KNS_KnessetDates` | תקופות כנסת — Knesset terms & sessions | 164 |

## File Structure

```
data/
  KNS_Person/
    manifest.yaml              # Schema, source, checksums
    KNS_Person_0.jsonl         # Data (up to 50K records per file)
  KNS_Bill/
    manifest.yaml
    KNS_Bill_0.jsonl
    KNS_Bill_1.jsonl
  ...
manifest.yaml                  # Root manifest with provenance
```

See `manifest.yaml` for checksums and record counts.
