# Example: auth-provider decision

Context:
Our Auth0 contract renews in four months. Enterprise SSO customers are asking for more flexible SAML configuration, and engineering has spent increasing time maintaining custom workarounds.

Options discussed:
1. Renew Auth0 and keep the existing configuration.
2. Move to WorkOS for enterprise SSO and user management.
3. Build a custom identity layer around our existing authentication setup.

Discussion:
Engineering believes WorkOS would reduce custom SAML maintenance and better support the FactSet federation work. Product wants to avoid delaying the enterprise roadmap. Finance noted WorkOS will cost more at our current scale, but the cost difference is manageable if it prevents further delivery delays.

Decision:
Move to WorkOS, beginning with enterprise SSO. Keep the existing login experience during migration.

Concerns:
Migration will require careful customer communication and a phased rollout. We do not yet know the full effort required for legacy user migration.

Owner:
Frontend Engineering Lead

Next action:
Engineering to produce a migration plan and effort estimate before the end of the month.