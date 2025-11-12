# GOV.UK Design System - Sublime Text Snippets

A complete collection of Sublime Text snippets for all GOV.UK Design System components.

## Installation

1. Copy all `.sublime-snippet` files to your Sublime Text Packages directory:
   - **macOS**: `~/Library/Application Support/Sublime Text/Packages/User/`
   - **Windows**: `%APPDATA%\Sublime Text\Packages\User\`
   - **Linux**: `~/.config/sublime-text/Packages/User/`

2. Restart Sublime Text

## Usage

Type the trigger keyword and press `Tab` to expand the snippet. Use `Tab` to navigate between placeholders.

## Available Snippets

### Navigation Components
- `govuk-back-link` - Back link component
- `govuk-breadcrumbs` - Breadcrumbs navigation
- `govuk-skip-link` - Skip to main content link
- `govuk-pagination` - Pagination controls

### Layout Components
- `govuk-header` - GOV.UK header with logo
- `govuk-footer` - GOV.UK footer
- `govuk-accordion` - Collapsible accordion sections
- `govuk-tabs` - Tabbed content interface

### Form Components
- `govuk-text-input` - Text input field
- `govuk-textarea` - Multi-line text area
- `govuk-select` - Dropdown select menu
- `govuk-radios` - Radio button group
- `govuk-checkboxes` - Checkbox group
- `govuk-date-input` - Date input (day/month/year)
- `govuk-file-upload` - File upload input
- `govuk-password-input` - Password input with show/hide toggle
- `govuk-character-count` - Textarea with character counter
- `govuk-fieldset` - Form fieldset wrapper

### Button Components
- `govuk-button` - Default button
- `govuk-button-secondary` - Secondary button
- `govuk-button-warning` - Warning button
- `govuk-button-start` - Start button with arrow icon
- `govuk-button-group` - Button group container

### Information Components
- `govuk-inset-text` - Highlighted inset text
- `govuk-warning-text` - Warning message with icon
- `govuk-details` - Expandable details/summary
- `govuk-notification-banner` - Notification banner
- `govuk-panel` - Confirmation panel
- `govuk-tag` - Status tag/label
- `govuk-summary-list` - Key-value summary list
- `govuk-table` - Data table
- `govuk-task-list` - Task list with status

### Error Handling
- `govuk-error-message` - Inline error message
- `govuk-error-summary` - Error summary at top of page

### Utility Components
- `govuk-phase-banner` - Alpha/Beta phase banner
- `govuk-cookie-banner` - Cookie consent banner

## Example Usage

1. Type `govuk-button` and press `Tab`
2. The button HTML will be inserted with placeholders
3. Type your button text and press `Tab` to move to the next placeholder
4. Continue tabbing through all placeholders to customize the component

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

- These snippets use the standard GOV.UK Design System HTML structure
- Make sure you have the GOV.UK Frontend CSS and JavaScript included in your project
- Some components require JavaScript initialization (data-module attributes are included)
