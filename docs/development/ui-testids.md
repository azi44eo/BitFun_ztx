# UI Test IDs

This document records stable `data-testid` values used by BitFun UI automation.
Test IDs are grouped by product area and should be added only when an automated
workflow needs a stable locator.

Rules:

- Use `data-testid` only as a test locator. Do not branch product logic on it.
- Prefer the real interactive element: `button`, `input`, editable region, or dialog root.
- Keep `data-testid` values stable, lowercase, and hyphen-separated.
- For repeated items, use one shared `data-testid` plus a stable data attribute.
- Do not use visible text, CSS classes, coordinates, screenshots, or XPath paths as primary locators.

## App Shell

| Element name | data-testid | Notes |
|---|---|---|
| App layout root | `app-layout` | App load-ready anchor. |
| Main content area | `app-main-content` | Primary scene content container. |
| Navigation panel | `nav-panel` | Left navigation container. |

## Navigation

| Element name | data-testid | Notes |
|---|---|---|
| Footer more button | `nav-footer-more-btn` | Opens the footer overflow menu. |
| Footer menu | `nav-footer-menu` | Overflow menu opened from the footer more button. |
| Footer settings item | `nav-footer-settings-item` | Opens the Settings scene from the footer menu. |
| Footer shell button | `nav-footer-shell-btn` | Opens or closes the shell scene nav. |
| Footer browser button | `nav-footer-browser-btn` | Opens browser scene or browser panel depending on active context. |
| Session nav item | `session-nav-item` | Repeated item. Pair with `data-session-id`. |
| Session nav show more | `session-nav-show-more` | Expands additional sessions. |

## Chat

| Element name | data-testid | Notes |
|---|---|---|
| Chat input container | `chat-input-container` | Root container for the composer. |
| Chat input editable region | `chat-input-textarea` | Rich text editable region. |
| Chat send button | `chat-input-send-btn` | Send action when input is valid. |
| Chat cancel button | `chat-input-cancel-btn` | Stop/cancel action while work is running. |
| Chat workspace strip | `chat-input-workspace-strip` | Shows current workspace context when present. |
| Chat target switcher | `chat-input-target-switcher` | Agent/target selector container. |
| Chat image strip | `chat-input-image-strip` | Attached image preview strip. |
| Chat boost start BTW | `chat-input-boost-start-btw` | Starts BTW/deep-review boost flow when available. |

## Settings

| Element name | data-testid | Notes |
|---|---|---|
| Settings scene root | `settings-scene` | Root content area for the Settings scene. Includes `data-settings-tab`. |
| Settings scene content | `settings-scene-content` | Active settings tab content wrapper. |
| Settings navigation root | `settings-nav` | Left-side settings navigation. |
| Settings navigation tab | `settings-nav-tab` | Repeated item. Pair with `data-settings-tab`. |

## Notifications

| Element name | data-testid | Notes |
|---|---|---|
| Notification button | `notification-button` | Opens or toggles the notification center. |
| Notification center dialog | `notification-center` | Notification center modal root. |
| Notification center close button | `notification-center-close-btn` | Closes the notification center. |
| Notification center active section | `notification-center-active-section` | Present only when active task notifications exist. |

## Background Activity

| Element name | data-testid | Notes |
|---|---|---|
| Pending queue panel | `pending-queue-panel` | Background/pending activity panel. |
| ACP plan panel | `acp-plan-panel` | ACP plan display panel. |
| Thread goal strip button | `thread-goal-strip-button` | Thread goal control in chat header/input region. |
| BTW session stop review | `btw-session-panel-stop-review` | Stops BTW review from the BTW panel. |
| BTW session origin button | `btw-session-panel-origin-button` | Returns to the origin session from BTW panel. |

## Flow Chat Header

| Element name | data-testid | Notes |
|---|---|---|
| Background activities button | `flowchat-header-background-activities` | Opens background activity state. |
| Pull requests button | `flowchat-header-pull-requests` | Opens pull request related UI. |
| Search bar | `flowchat-header-search-bar` | Header search container. |
| Search input/action | `flowchat-header-search` | Header search control. |
| Turn list | `flowchat-header-turn-list` | Turn navigation list. |
| Previous turn button | `flowchat-header-turn-prev` | Moves to previous matched/visible turn. |
| Next turn button | `flowchat-header-turn-next` | Moves to next matched/visible turn. |

## Markdown Inline AI

| Element name | data-testid | Notes |
|---|---|---|
| Inline AI panel | `md-inline-ai-panel` | Markdown inline AI panel root. |
| Inline AI input | `md-inline-ai-input` | Prompt input for inline AI. |
| Inline AI continue action | `md-inline-ai-continue` | Continue-writing quick action. |
| Inline AI summary action | `md-inline-ai-summary` | Summary quick action. |
| Inline AI todo action | `md-inline-ai-todo` | Todo-generation quick action. |
| Inline AI preview | `md-inline-ai-preview` | Preview block root. |
| Inline AI preview content | `md-inline-ai-preview-content` | Rendered preview content. |
| Inline AI preview placeholder | `md-inline-ai-preview-placeholder` | Streaming placeholder. |
| Inline AI preview error | `md-inline-ai-preview-error` | Preview error message. |
| Inline AI accept button | `md-inline-ai-accept` | Accepts inline AI output. |
| Inline AI reject button | `md-inline-ai-reject` | Rejects inline AI output. |
| Inline AI retry button | `md-inline-ai-retry` | Retries inline AI output. |

