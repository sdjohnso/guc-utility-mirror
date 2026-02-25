# GUC Utility Mirror

Structured JSON mirror of Greenville Utilities Commission capital projects.

## Structure

```
projects/       # One JSON file per project (WCP, SCP, ECP, GCP)
extractions/    # Raw extraction outputs by meeting date
```

## Schema

See any project file for full schema. Key fields:
- `project_id`, `project_type`, `project_name`
- `budget.current_amount`, `budget.amendments[]`
- `location.centroid`, `location.street_references`
- `status`, `completion_target`
- `meeting_references[]`

## Update Schedule

Updated monthly after GUC Board meetings (3rd Thursday).

**Source:** https://www.guc.com/about-us/agendas-and-minutes
