# Engineering Contribution Standard

This repository uses review-driven engineering and intentionally avoids personal-information requirements.

## Change classification
Classify work as patch, compatible feature, breaking change, security change, or operational change. Breaking changes require migration and rollback notes.

## Quality requirements
Preserve explicit interfaces, bounded validation, deterministic behavior, safe error handling, least privilege, no embedded secrets and sufficient observability for technical diagnosis.

## Documentation changes
Documentation must avoid publishing private contact information, precise location, credentials, personal identifiers, production-only endpoints or sensitive infrastructure details.

## Testing and verification
Executable changes should cover success, malformed input, boundaries, dependency failure and regression cases. Documentation changes must be checked for broken links, accidental secrets and private-data exposure.

## Review gate
Do not merge while compatibility, security/privacy impact, verification method or rollback expectations are unknown.
