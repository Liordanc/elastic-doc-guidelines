# Writing about the UI

Guidelines for documenting user interfaces and interactions.

## General principles

- Describe use cases, not piece-by-piece UI
- Write steps for complex actions only
- Keep procedures between 5-9 steps
- Use active voice
- Match UI element capitalization exactly
- Use **bold** for component names and buttons
- Use *italic x* for variable text in component names
- Test all procedures before publishing

## UI component language

| Component | Guidance | Example |
|---|---|---|
| Button | Use "click" for action, "select" for choice | Click **Save** to confirm |
| Checkbox | Use "select" and "clear", not "check"/"uncheck" | Select the **Enable HTTPS** checkbox |
| Radio button | Use "select" | Select the **Production** option |
| Text field | Use "enter" for action | In the **Name** field, enter a unique identifier |
| Toggle/Switch | Refer to as "toggle" | Toggle the **SSL** setting |
| Dropdown | Use "select" | From the **Status** dropdown, select **Active** |
| Menu | Use "From the menu" or "select", not "open/close" | From the actions menu, select **Delete** |
| Link | Use "select" or "click" | Select the **Learn more** link |
| Tab | Use "select" | Select the **Overview** tab |
| Icon | Refer by icon or tooltip name | Click the settings icon |

## Verbs: Select vs. Click

- **Use "select"** for making choices: Select an option, toggle a state, pick from a list
- **Use "click"** for taking action: Click a button, click a link, click an icon

## Prepositions with UI elements

| Preposition | Use with | Example |
|---|---|---|
| in | Field, section, pane, table, window, menu bar | In the **Name** field |
| on | Page, screen, tab, toolbar | On the **Dashboard** page |
| from | Menu, dropdown, list | From the **Actions** menu |
| at | Command prompt | At the command prompt |

## Screenshots

### When to use screenshots
- For complex UI that's hard to describe
- For introductions
- For time-bound docs (highlights, blog posts)

### Best practices
- Use 16:9 aspect ratio (1366x768px)
- Capture only essential UI elements
- Avoid navigation, breadcrumbs, header when possible
- Add border for definition
- Use Elastic brand colors for annotations (pink: #F04E98)
- Anonymize sensitive data
- Use GIFs only if they're under 15 seconds

## Referring to apps and pages

- "Find **APP** in the navigation menu or use the global search field"
- "Open **APP or PAGE** by searching in the global search field"
- Be flexible: users may access features different ways

## Icon buttons

- Include the icon inline to reinforce interaction
- Use the tooltip text as the name
- Example: "Click the refresh icon to reload the page"

## Naming UI conventions

- **Global header**: Top bar with global controls and search
- **Navigation menu**: Primary navigation on the left
- **Solution view**: Setting that controls navigation menu content
- **Secondary navigation**: Panel for sub-items
- **Application menu**: Bar above workspace for app-specific actions
- **Workspace**: Main content area
- **Flyout**: Panel sliding from the right
- **Sidebar**: Global right-hand panel for plugins
