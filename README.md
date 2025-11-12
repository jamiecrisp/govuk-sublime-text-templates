# GOV.UK Design System - Sublime Text Snippets

A complete collection of Sublime Text snippets for all GOV.UK Design System components.

This package includes **two versions** of snippets:
- **HTML snippets** (`govuk-*`) - Plain HTML markup (36 snippets)
- **Nunjucks snippets** (`govuk-njk-*`) - Nunjucks macro templates (35 snippets)

## Installation

1. Copy all `.sublime-snippet` files to your Sublime Text Packages directory:
   - **macOS**: `~/Library/Application Support/Sublime Text/Packages/User/`
   - **Windows**: `%APPDATA%\Sublime Text\Packages\User\`
   - **Linux**: `~/.config/sublime-text/Packages/User/`

2. Restart Sublime Text

## Usage

Type the trigger keyword and press `Tab` to expand the snippet. Use `Tab` to navigate between placeholders.

### Choosing Between HTML and Nunjucks

- **Use Nunjucks snippets** (`govuk-njk-*`) if you're building a GOV.UK service with Node.js and the GOV.UK Frontend Nunjucks macros
- **Use HTML snippets** (`govuk-*`) if you're working with plain HTML or another templating system

### Examples

**Nunjucks:**
```
govuk-njk-button → {% from "govuk/components/button/macro.njk" import govukButton %}...
```

**HTML:**
```
govuk-button → <button type="submit" class="govuk-button"...
```

## Available Snippets

All components are available in both HTML and Nunjucks formats. Add `-njk-` for Nunjucks versions (e.g., `govuk-njk-button`).

### Navigation Components
- `govuk-back-link` / `govuk-njk-back-link` - Back link component
- `govuk-breadcrumbs` / `govuk-njk-breadcrumbs` - Breadcrumbs navigation
- `govuk-skip-link` / `govuk-njk-skip-link` - Skip to main content link
- `govuk-pagination` / `govuk-njk-pagination` - Pagination controls

### Layout Components
- `govuk-header` / `govuk-njk-header` - GOV.UK header with logo
- `govuk-footer` / `govuk-njk-footer` - GOV.UK footer
- `govuk-accordion` / `govuk-njk-accordion` - Collapsible accordion sections
- `govuk-tabs` / `govuk-njk-tabs` - Tabbed content interface

### Form Components
- `govuk-text-input` / `govuk-njk-input` - Text input field
- `govuk-textarea` / `govuk-njk-textarea` - Multi-line text area
- `govuk-select` / `govuk-njk-select` - Dropdown select menu
- `govuk-radios` / `govuk-njk-radios` - Radio button group
- `govuk-checkboxes` / `govuk-njk-checkboxes` - Checkbox group
- `govuk-date-input` / `govuk-njk-date-input` - Date input (day/month/year)
- `govuk-file-upload` / `govuk-njk-file-upload` - File upload input
- `govuk-password-input` / `govuk-njk-password-input` - Password input with show/hide toggle
- `govuk-character-count` / `govuk-njk-character-count` - Textarea with character counter
- `govuk-fieldset` / `govuk-njk-fieldset` - Form fieldset wrapper

### Button Components
- `govuk-button` / `govuk-njk-button` - Default button
- `govuk-button-secondary` / `govuk-njk-button-secondary` - Secondary button
- `govuk-button-warning` / `govuk-njk-button-warning` - Warning button
- `govuk-button-start` / `govuk-njk-button-start` - Start button with arrow icon
- `govuk-button-group` - Button group container (HTML only)

### Information Components
- `govuk-inset-text` / `govuk-njk-inset-text` - Highlighted inset text
- `govuk-warning-text` / `govuk-njk-warning-text` - Warning message with icon
- `govuk-details` / `govuk-njk-details` - Expandable details/summary
- `govuk-notification-banner` / `govuk-njk-notification-banner` - Notification banner
- `govuk-panel` / `govuk-njk-panel` - Confirmation panel
- `govuk-tag` / `govuk-njk-tag` - Status tag/label
- `govuk-summary-list` / `govuk-njk-summary-list` - Key-value summary list
- `govuk-table` / `govuk-njk-table` - Data table
- `govuk-task-list` / `govuk-njk-task-list` - Task list with status

### Error Handling
- `govuk-error-message` / `govuk-njk-error-message` - Inline error message
- `govuk-error-summary` / `govuk-njk-error-summary` - Error summary at top of page

### Utility Components
- `govuk-phase-banner` / `govuk-njk-phase-banner` - Alpha/Beta phase banner
- `govuk-cookie-banner` / `govuk-njk-cookie-banner` - Cookie consent banner

## Example Usage

### HTML Snippets
1. Type `govuk-button` and press `Tab`
2. The button HTML will be inserted with placeholders
3. Type your button text and press `Tab` to move to the next placeholder
4. Continue tabbing through all placeholders to customize the component

### Nunjucks Snippets
1. Type `govuk-njk-button` and press `Tab`
2. The Nunjucks macro import and call will be inserted
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

