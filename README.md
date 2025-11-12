# GOV.UK Design System - Sublime Text Snippets

A complete collection of Sublime Text snippets for all GOV.UK Design System components.

This package includes **two versions** of snippets:
- **HTML snippets** (`gds-*`) - Plain HTML markup (36 snippets)
- **Nunjucks snippets** (`gds-njk-*`) - Nunjucks macro templates (35 snippets)

## Installation

1. Copy all `.sublime-snippet` files to your Sublime Text Packages directory:
   - **macOS**: `~/Library/Application Support/Sublime Text/Packages/User/`
   - **Windows**: `%APPDATA%\Sublime Text\Packages\User\`
   - **Linux**: `~/.config/sublime-text/Packages/User/`

2. Restart Sublime Text

## Usage

Type the trigger keyword and press `Tab` to expand the snippet. Use `Tab` to navigate between placeholders.

### Choosing Between HTML and Nunjucks

- **Use Nunjucks snippets** (`gds-njk-*`) if you're building a GOV.UK service with Node.js and the GOV.UK Frontend Nunjucks macros
- **Use HTML snippets** (`gds-*`) if you're working with plain HTML or another templating system

### Examples

**Nunjucks:**
```
gds-njk-button → {{ govukButton({ text: "Save and continue" }) }}
```

**HTML:**
```
gds-button → <button type="submit" class="govuk-button"...
```

## Available Snippets

All components are available in both HTML and Nunjucks formats. Add `-njk-` for Nunjucks versions (e.g., `gds-njk-button`).

### Navigation Components
- `gds-back-link` / `gds-njk-back-link` - Back link component
- `gds-breadcrumbs` / `gds-njk-breadcrumbs` - Breadcrumbs navigation
- `gds-skip-link` / `gds-njk-skip-link` - Skip to main content link
- `gds-pagination` / `gds-njk-pagination` - Pagination controls

### Layout Components
- `gds-header` / `gds-njk-header` - GOV.UK header with logo
- `gds-footer` / `gds-njk-footer` - GOV.UK footer
- `gds-accordion` / `gds-njk-accordion` - Collapsible accordion sections
- `gds-tabs` / `gds-njk-tabs` - Tabbed content interface

### Form Components
- `gds-text-input` / `gds-njk-input` - Text input field
- `gds-textarea` / `gds-njk-textarea` - Multi-line text area
- `gds-select` / `gds-njk-select` - Dropdown select menu
- `gds-radios` / `gds-njk-radios` - Radio button group
- `gds-checkboxes` / `gds-njk-checkboxes` - Checkbox group
- `gds-date-input` / `gds-njk-date-input` - Date input (day/month/year)
- `gds-file-upload` / `gds-njk-file-upload` - File upload input
- `gds-password-input` / `gds-njk-password-input` - Password input with show/hide toggle
- `gds-character-count` / `gds-njk-character-count` - Textarea with character counter
- `gds-fieldset` / `gds-njk-fieldset` - Form fieldset wrapper

### Button Components
- `gds-button` / `gds-njk-button` - Default button
- `gds-button-secondary` / `gds-njk-button-secondary` - Secondary button
- `gds-button-warning` / `gds-njk-button-warning` - Warning button
- `gds-button-start` / `gds-njk-button-start` - Start button with arrow icon
- `gds-button-group` - Button group container (HTML only)

### Information Components
- `gds-inset-text` / `gds-njk-inset-text` - Highlighted inset text
- `gds-warning-text` / `gds-njk-warning-text` - Warning message with icon
- `gds-details` / `gds-njk-details` - Expandable details/summary
- `gds-notification-banner` / `gds-njk-notification-banner` - Notification banner
- `gds-panel` / `gds-njk-panel` - Confirmation panel
- `gds-tag` / `gds-njk-tag` - Status tag/label
- `gds-summary-list` / `gds-njk-summary-list` - Key-value summary list
- `gds-table` / `gds-njk-table` - Data table
- `gds-task-list` / `gds-njk-task-list` - Task list with status

### Error Handling
- `gds-error-message` / `gds-njk-error-message` - Inline error message
- `gds-error-summary` / `gds-njk-error-summary` - Error summary at top of page

### Utility Components
- `gds-phase-banner` / `gds-njk-phase-banner` - Alpha/Beta phase banner
- `gds-cookie-banner` / `gds-njk-cookie-banner` - Cookie consent banner

## Example Usage

### HTML Snippets
1. Type `gds-button` and press `Tab`
2. The button HTML will be inserted with placeholders
3. Type your button text and press `Tab` to move to the next placeholder
4. Continue tabbing through all placeholders to customize the component

### Nunjucks Snippets
1. Type `gds-njk-button` and press `Tab`
2. The Nunjucks macro call will be inserted
3. Tab through placeholders to customize the button text and options
4. The macro automatically handles accessibility and proper markup

## Customization

All snippets include tab stops (`${1:placeholder}`) to help you quickly customize:
- IDs and names
- Label text
- Hint text
- Values
- Links

## Resources

- [GOV.UK Design System](https://design-system.service.gov.uk/)
- [GOV.UK Frontend](https://github.com/alphagov/govuk-frontend)

## Notes

### HTML Snippets
- Use the standard GOV.UK Design System HTML structure
- Make sure you have the GOV.UK Frontend CSS and JavaScript included in your project

### Nunjucks Snippets
- Require GOV.UK Frontend to be installed: `npm install govuk-frontend`
- Configure your Nunjucks paths to include `node_modules/govuk-frontend/dist`

