# Data Model

## Sponsor

| Field | Type | Description |
|---|---|---|
| sponsor_id | string | Unique sponsor identifier |
| company_name | string | Sponsor/company name |
| sector | string | Industry or business category |
| priority | enum | low, medium, high, strategic |
| fit_score | number | 1–10 sponsor fit |
| status | enum | new, contacted, interested, negotiating, committed, rejected, dormant |
| package_target | string | Target sponsorship package |
| cash_value | number | Expected or committed cash value |
| in_kind_value | number | Expected or committed in-kind value |
| owner | string | Team member responsible |
| next_action | string | Next required action |
| next_action_date | date | Follow-up date |
| notes | string | Context and relationship notes |

## Contact

| Field | Type | Description |
|---|---|---|
| contact_id | string | Unique contact identifier |
| sponsor_id | string | Related sponsor |
| full_name | string | Contact name |
| job_title | string | Contact title |
| email | string | Contact email |
| phone | string | Contact phone |
| linkedin_url | string | LinkedIn profile |
| relationship_source | string | Warm intro, cold outreach, existing relationship, etc. |

## Visibility Item

| Field | Type | Description |
|---|---|---|
| item_id | string | Unique visibility item |
| sponsor_id | string | Related sponsor |
| item_type | enum | backdrop, banner, social, booth, stage mention, logo, product placement, hospitality |
| description | string | Visibility description |
| delivery_status | enum | pending, in_progress, delivered, blocked |
| proof_url | string | Link to image, post, or document proof |
