# Pydantic-V2
Pydantic v2 — validators, computed fields, nested models, and serialization.

## What's Covered

| File | Concept | What It Shows |
|------|---------|---------------|
| `1_pydantic_why.py` | BaseModel & Field | Type enforcement, `EmailStr`, `AnyUrl`, `Annotated` constraints, strict mode |
| `2_field_validator.py` | Field Validators | Custom per-field validation logic, domain whitelisting, value transforms |
| `3_model_validator.py` | Model Validators | Cross-field validation (e.g., age-based emergency contact rule) |
| `4_computed_fields.py` | Computed Fields | Deriving new fields (BMI) from existing ones at validation time |
| `5_nested_models.py` | Nested Models | Composing models (`Address` inside `Patient`), `model_dump` with filters |
| `6_serialization.py` | Serialization | `model_dump()` with `exclude_unset`, default field handling |

---

## Skills Demonstrated

- **Data validation** with runtime type coercion and strict mode
- **Custom validators** using `@field_validator` and `@model_validator`
- **Computed properties** with `@computed_field`
- **Nested model composition** and structured serialization
- **Real-world constraints**: email domains, URL types, list length limits, cross-field rules

---

## Getting Started

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/pydantic-v2.git
cd pydantic-v2

# Install dependencies
pip install pydantic[email]

# Run any script
python 1_pydantic_why.py
python 2_field_validator.py
# ... and so on
```

**Python version:** 3.10+  
**Pydantic version:** v2.x

---

## Why Pydantic

Pydantic is used under the hood by **FastAPI**, **LangChain**, **LlamaIndex**, and dozens of other frameworks. Understanding it deeply means you can build more reliable APIs, define cleaner AI agent schemas, and catch data bugs before they hit production.

---

## Repo Structure

```
pydantic-v2/
├── 1_pydantic_why.py         # BaseModel fundamentals
├── 2_field_validator.py      # Per-field validation
├── 3_model_validator.py      # Cross-field validation
├── 4_computed_fields.py      # Derived fields
├── 5_nested_models.py        # Model composition
└── 6_serialization.py        # Serialization control
```
