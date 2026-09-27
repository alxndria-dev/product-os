# Example: ambiguous confirmation modal

Context:
A user clicks “Delete workspace”.

A modal appears with:
- Heading: “Delete workspace?”
- Text: “This cannot be undone.”
- Secondary button: “Cancel”
- Primary red button: “Delete”

The workspace can contain saved research, notes, and shared collaborators.

No further detail is supplied.

Open questions:
- Does deleting remove content for every collaborator?
- Can a workspace be restored?
- What happens if the user only has permission to edit, not delete?
- Is deleting a workspace meaningfully different from leaving it?