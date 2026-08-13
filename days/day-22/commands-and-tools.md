# 🛠️ Tools / Practical Commands — Day 22

> Use only synthetic classroom environments. Never run commands against systems you do not own
> or have explicit authorization to assess.

## Git
```bash
git clone <your-repository>
cd GRC-Zero-to-Hero
git status
git pull
```

## Search curriculum
```bash
find days -name "README.md" | sort
find templates -type f | sort
```

## CSV inspection with Python
```bash
python -c "import csv; print(list(csv.reader(open('templates/risk-register.csv')))[:3])"
```

## Evidence hygiene
```text
PUBLIC REPO
  ├── synthetic data ✅
  ├── dummy identifiers ✅
  └── training evidence ✅

NEVER COMMIT
  ├── passwords ❌
  ├── API keys ❌
  ├── customer PII ❌
  ├── production logs ❌
  └── confidential audit evidence ❌
```

## Tool thinking
A tool is useful only when the underlying process, ownership, control and evidence model are
defined. Do not confuse tool output with assurance.
