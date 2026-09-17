# Security Policy

## Public portfolio scope

This repository contains sanitized demonstration workflows only. It must never
contain production credentials, tokens, secrets, internal endpoints, customer
identifiers, tenant IDs, workspace IDs, dataset IDs or confidential business
rules.

## Reporting a problem

Do not publish secrets or sensitive evidence in a public issue. Contact the
repository owner privately through the GitHub profile and include only the
minimum information necessary to identify the problem.

## Credential handling

Production implementations should:

- store secrets in the n8n credential manager or environment variables;
- apply least-privilege access;
- separate public demonstrations from private production workflows;
- rotate any credential that has been exposed in an export or commit;
- scan staged files before every push.

The JSON files in this repository use placeholders and contain no operational
credentials.
