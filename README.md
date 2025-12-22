# Spool Support Sync - License Database

This repository contains license files for Spool Support Sync customers.

## File Format

Each license is stored as `{license-id}.json` with the following structure:

- `license_id`: Unique identifier
- `customer_name`: Customer name
- `customer_email`: Customer email
- `license_type`: trial/standard/professional/enterprise
- `expiration_date`: ISO format date (null for perpetual)
- `max_operations`: Operation limit (null for unlimited)
- `revoked`: Boolean indicating if license is revoked
- `revoke_reason`: Reason for revocation (if applicable)

## License Status

- ✅ Active: License is valid and usable
- ❌ Revoked: License has been revoked
- ⏰ Expired: License expiration date has passed
