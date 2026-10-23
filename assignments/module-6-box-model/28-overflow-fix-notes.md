# Assignment 28: Overflow Fix Notes

The `before` page intentionally uses a fixed-width layout, an oversized panel, an unbroken string, and a fixed-height note. The corrected page demonstrates these changes:

- Use `width: min(100%, ...)` and flexible columns so the page fits its container.
- Add `min-width: 0` and `box-sizing: border-box` to prevent flex children from forcing extra width.
- Keep media within its card with `max-width: 100%`.
- Let long text wrap with `overflow-wrap: anywhere`.
- Let a text box grow with its content instead of clipping it at a fixed height.
- Put a wide table in its own horizontal scrolling container.
