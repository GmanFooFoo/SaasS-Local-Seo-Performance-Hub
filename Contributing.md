#!/bin/bash
# setup_local_seo_repo.sh
# Script to create the initial folder structure for Local SEO Performance Hub (business docs only)

# Root folder
mkdir -p local-seo-performance-hub
cd local-seo-performance-hub || exit

# Main folders
mkdir -p docs assets/logos assets/pitch_deck assets/screenshots

# Create README
cat << 'EOF' > README.md
# Local SEO Performance Hub – MVP

## Overview
This repository contains the **business development and documentation** for the MVP of the Local SEO Performance Hub SaaS project.

👉 This repo does not contain production code yet. It focuses on:
- MVP specification
- Business plan
- Growth strategy
- Competitor analysis
- Compliance considerations
- Roadmap and milestones
EOF

# Create documentation files
cat << 'EOF' > docs/mvp_specification.md
# MVP Specification – Local SEO Performance Hub
(See full spec document)
EOF

cat << 'EOF' > docs/business_plan.md
# Business Plan
- Monetization model
- Pricing tiers
- Revenue projections
EOF

cat << 'EOF' > docs/growth_strategy.md
# Growth Strategy
- ICP (ideal customer profile)
- Free scan funnel
- Content & partnerships
EOF

cat << 'EOF' > docs/competitor_analysis.md
# Competitor Analysis
- BrightLocal
- BirdEye
- Yext
- Other tools
EOF

cat << 'EOF' > docs/compliance_notes.md
# Compliance Notes
- GDPR considerations
- API usage restrictions
- International differences (EU vs US market)
EOF

cat << 'EOF' > docs/roadmap.md
# Roadmap
## Phase 1 – MVP
## Phase 2 – Feature expansion
## Phase 3 – Agency mode
## Phase 4 – Internationalization
EOF

# Gitignore
cat << 'EOF' > .gitignore
# Ignore system files
.DS_Store
Thumbs.db

# Ignore temporary files
*.tmp
*.bak

# Ignore design software files
assets/**/*.psd
assets/**/*.ai
EOF

echo "✅ Local SEO Performance Hub repo structure created successfully."
