# Example: data table and filters

Context:
A company screener contains:

- A filter bar with sector, country, market cap, and “has recent research” filters
- An Apply filters button
- A Reset button
- A sortable table of company results
- A row action to save a company to a workspace

The desktop design shows five filters in one horizontal row. The results table contains ten columns, including company name, sector, market cap, revenue growth, research count, and last updated.

Interaction notes:
Filters should update the table only after users select Apply filters.
Rows can be selected, but no bulk action is shown.

No behaviour is defined for:
- Small screens
- Long company names
- No results
- Filter loading
- Sort direction or persistence
- Saved-company confirmation
- Keyboard interaction