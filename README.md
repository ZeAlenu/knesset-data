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

## File Structure

```
data/
  KNS_Person/
    KNS_Person-000001.jsonl    # IDs 0–9,999
    KNS_Person-000002.jsonl    # IDs 10,000–19,999
  KNS_Bill/
    ...
schema/v1/schema.json          # Schema for all entities
manifest.yaml                  # SHA-256 checksums + metadata
```

Each entity is stored under `data/{entity}/` as partitioned JSONL files (10,000 IDs per partition).
See `manifest.yaml` for checksums and record counts.

## Contributing

Data is auto-generated from the Knesset API. To report issues, open a GitHub issue.
