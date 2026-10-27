# KM Authoring & Contribution Guide

## How to Create a New Knowledge Asset
1. Copy the raw layout from `km/templates/ARTICLE_TEMPLATE.md`.
2. Save your new file in the appropriate domain folder inside `km/knowledge-base/` (e.g., `km/knowledge-base/erp-systems/`).
3. Fill out the required YAML header at the top of the file, ensuring all tags exist in `km/governance/TAXONOMY.md`.
4. Set the document status to `Draft`.

## Document Review & Verification
* Submit a review request to the designated functional owner.
* Once verified for accuracy, update the `status` field in the header from `Draft` to `Verified` and set the `last_reviewed` date.
