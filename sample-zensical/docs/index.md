This page demonstrates a broad set of commonly used Confluence-compatible components in clean HTML, organized as a practical reference for building rich, scannable documentation.

!!! info "Info"
    **Purpose:** Use this page as a visual sample for page structure, formatting patterns, callouts, lists, tables, layouts, links, statuses, code blocks, quotes, tasks, decisions, media, and expandable content.

# Core text and inline formatting

This paragraph shows **bold**, _italic_, <ins>underline</ins>, strikethrough, `inline code`, subscript, superscript, and ==highlighted text==.

It also includes ==text color==, a standard [hyperlink](https://www.atlassian.com), a [https://www.atlassian.com](https://www.atlassian.com), a status lozenge <mark style="background-color:rgba(76, 175, 80, 0.3); padding: 0.2em;">Ready</mark>, and an emoji :rocket: 

This is a centered paragraph.

This paragraph is indented one level.

This paragraph uses the small font style.

* * *

# Panels and callouts

!!! info "Info"
    **Info panel:** Use for helpful explanatory content and important background.

!!! note "Note"
    **Note panel:** Use for supporting context, clarifications, or references.

!!! note "Note"
    **Warning panel:** Use when the reader should take care before proceeding.

!!! tip "Tip"
    **Success panel:** Use to highlight a good outcome, completion, or confirmation.

!!! warning "Warning"
    **Error panel:** Use for critical issues, blockers, or failures that need attention.

!!! quote "Quote"
    **Custom panel:** Use when you want a tailored visual treatment for a special message.

# Lists, tasks, and decisions

## Bullet and numbered lists

- First bullet item

- Second bullet item
    
    - Nested bullet item


- Third bullet item


<!--THE END-->

1. First numbered item

2. Second numbered item

3. Third numbered item


## Task list

 - [x]   Draft content complete
 - [ ]   Review formatting
 - [ ]   Publish page

## Block tasks

 - [x]   Create showcase sections
 - [ ]   Validate component rendering in target space

## Decision list

 - [x]   Use panels to surface important guidance.
 - [ ]   Add space-specific branding examples.

# Table examples

| Component | Purpose                      | Best use                        | Status                                                                                         |
|-----------|------------------------------|---------------------------------|------------------------------------------------------------------------------------------------|
| Panel     | Highlights important content | Warnings, notes, summaries      | <mark style="background-color:rgba(33, 150, 243, 0.3); padding: 0.2em;">Active</mark>          |
| Table     | Structures information       | Comparison, reference, tracking | <mark style="background-color:rgba(76, 175, 80, 0.3); padding: 0.2em;">Recommended</mark>      |
| Expand    | Hides secondary detail       | FAQs, optional guidance         | <mark style="background-color:rgba(255, 235, 59, 0.3); padding: 0.2em;">Use selectively</mark> |

## Table with nested content

| Area      | Example content                                     | Details                                                                               |
|-----------|-----------------------------------------------------|---------------------------------------------------------------------------------------|
| Callout   | !!! note "Note"<br />    Panel inside a table cell. | ??? question "Show detail"<br />    Nested expands are supported inside table cells.  |
| Reference | > Blockquotes can also appear in table cells.       | - Useful for compact examples
<br />- Keeps the page scannable
 |

# Layouts and columns

!!! info "Info"
    **Left column**
    
    Use columns for side-by-side comparisons, summaries, or paired content.

!!! tip "Tip"
    **Right column**
    
    Columns work well for dashboards, quick references, and visual balance.

**Column 1**  
Short summary content.

**Column 2**  
Another concise content block.

**Column 3**  
Useful for grouped highlights.

# Expandable sections

??? question "Standard expand"
    Use expands to keep long pages easy to scan while still preserving detailed reference information.
    
    - Good for FAQs

    - Good for troubleshooting notes

    - Good for advanced examples


??? question "Wide expand"
    This expand demonstrates breakout behavior for content that benefits from additional width.

# Quotes, code, and media

> Well-structured pages are easier to read, easier to maintain, and more useful over time.

```html
<div data-type="panel-info"><p>Example panel content</p></div>
```
```json
{
  "component": "status",
  "color": "green",
  "label": "Ready"
}
```

Example external image:

`https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=800&q=80`

Example embed card:

`https://www.youtube.com/watch?v=dQw4w9WgXcQ`

# Links and cards

- [https://www.atlassian.com/software/confluence](https://www.atlassian.com/software/confluence)

- [https://developer.atlassian.com](https://developer.atlassian.com)


# Reference checklist

 - [x]   Headings and paragraphs
 - [x]   Inline formatting
 - [x]   Panels
 - [x]   Lists, tasks, and decisions
 - [x]   Tables
 - [x]   Layouts and columns
 - [x]   Expand sections
 - [x]   Quotes and code blocks
 - [x]   Images and embeds
 - [x]   Smart links and block cards

!!! note "Note"
    **Note on tabs:** Native tab components are not part of the supported HTML patterns available here. Use layouts, expands, tables, or linked child pages to create a tab-like reading experience.