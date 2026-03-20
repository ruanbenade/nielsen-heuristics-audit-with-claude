# Nielsen's 10 Usability Heuristics — Reference Guide

Detailed definitions, what to look for in screenshots, and common violation patterns for each heuristic.

---

## H1 — Visibility of System Status

**Definition:** The system should always keep users informed about what is going on, through appropriate feedback within reasonable time.

**What to look for in screenshots:**
- Loading states, spinners, progress bars, progress indicators
- Active/selected state indicators (which tab is active, which step you're on)
- Form submission feedback (success, processing, sent)
- Upload or download progress
- Notifications or badges indicating unread items
- Current location indicators in multi-step flows

**Common violations:**
- No loading indicator during operations
- No confirmation that an action (save, submit, send) was completed
- Active navigation item not visually differentiated
- No progress indicator in multi-step forms or wizards
- Ambiguous button states (does this button toggle on or off?)

---

## H2 — Match Between System and the Real World

**Definition:** The system should speak the users' language, with words, phrases, and concepts familiar to the user, rather than system-oriented terms. Follow real-world conventions.

**What to look for in screenshots:**
- Labels and terminology — are they plain language or jargon?
- Icons — are they universally understood or ambiguous?
- Metaphors — do they map to real-world concepts naturally?
- Date/time formats — do they match the user's locale expectations?
- Error messages — are they written in human language?

**Common violations:**
- Technical error codes exposed to users (e.g. "Error 403", "NullPointerException")
- System or developer terminology in labels (e.g. "Initialise", "Query", "Boolean")
- Icons without labels that are ambiguous or culturally specific
- Abbreviations that aren't universally understood
- Numeric IDs exposed where a name would be more meaningful

---

## H3 — User Control and Freedom

**Definition:** Users often choose system functions by mistake and will need a clearly marked "emergency exit" to leave the unwanted state without having to go through an extended dialogue.

**What to look for in screenshots:**
- Cancel buttons on forms, modals, and dialogs
- Back/undo options
- Close buttons on overlays and modals
- Clear ways to exit flows or processes
- Ability to edit or reverse recent actions

**Common violations:**
- Modal or overlay with no visible close/cancel option
- Multi-step flow with no back button
- Destructive actions (delete, submit) with no confirmation or undo
- Form that cannot be abandoned without data loss warning
- No way to return to a previous state

---

## H4 — Consistency and Standards

**Definition:** Users should not have to wonder whether different words, situations, or actions mean the same thing. Follow platform conventions.

**What to look for in screenshots:**
- Visual consistency — do similar elements look the same across the screen?
- Interaction consistency — do similar controls behave the same way?
- Terminology consistency — is the same concept always called the same thing?
- Platform conventions — does the UI follow iOS, Android, or web conventions as appropriate?
- Button hierarchy — is primary/secondary/tertiary button styling consistent?

**Common violations:**
- Two buttons that do similar things but look different
- Inconsistent use of capitalisation in labels
- Same action called different names in different places
- Primary action button sometimes on left, sometimes on right
- Inconsistent icon style (some outlined, some filled)
- Deviating from established platform patterns without good reason

---

## H5 — Error Prevention

**Definition:** Even better than good error messages is a careful design which prevents a problem from occurring in the first place.

**What to look for in screenshots:**
- Confirmation dialogs before destructive or irreversible actions
- Input constraints (date pickers instead of free text, dropdowns instead of open fields)
- Inline validation or format guidance on forms
- Disabled states that prevent premature submission
- Clear labelling of required vs optional fields
- Warnings before data loss

**Common violations:**
- Delete or submit buttons without confirmation step
- Free text input where a constrained input type would prevent errors
- No format guidance on fields with specific requirements (phone, date, postcode)
- Submit button active before required fields are complete
- No warning when navigating away from unsaved work

---

## H6 — Recognition Rather Than Recall

**Definition:** Minimise the user's memory load by making objects, actions, and options visible. The user should not have to remember information from one part of the interface to another.

**What to look for in screenshots:**
- Navigation — can users see where they can go from here?
- Labels on icons (or tooltips indicated)
- Visible options rather than hidden menus
- Context retained across screens (e.g. what was selected earlier)
- Search — is there autocomplete, suggestions, or recent searches?
- Form labels visible when fields are filled (not disappearing placeholder text)

**Common violations:**
- Icon-only navigation with no labels
- Placeholder text used as the only label (disappears on input)
- Options hidden behind unlabelled icons or gestures
- User required to remember information from a previous screen
- No breadcrumbs or context in deep navigation structures
- Hamburger menus that hide all navigation options

---

## H7 — Flexibility and Efficiency of Use

**Definition:** Accelerators — unseen by the novice user — may often speed up the interaction for the expert user such that the system can cater to both inexperienced and experienced users.

**What to look for in screenshots:**
- Keyboard shortcuts indicated (often in tooltips or menus)
- Saved preferences or recently used items
- Bulk actions for power users
- Customisable views or layouts
- Quick-access or pinned items
- Type-ahead / autocomplete

**Note:** This heuristic is often not fully assessable from a single static screenshot. Flag what you can observe and recommend user testing for the rest.

**Common violations:**
- No shortcuts or accelerators for frequent tasks
- Forced step-by-step flows with no way to skip known steps
- No way to save or reuse common inputs
- Repetitive tasks with no batch processing option

---

## H8 — Aesthetic and Minimalist Design

**Definition:** Dialogues should not contain irrelevant or rarely needed information. Every extra unit of information in a dialogue competes with the relevant units of information and diminishes their relative visibility.

**What to look for in screenshots:**
- Visual hierarchy — is the most important information most prominent?
- Clutter — is there content, labels, or UI elements that don't serve the current task?
- Whitespace — is there breathing room or is the screen packed?
- Secondary information — is it visually subordinate to primary content?
- Decoration — is any decoration adding noise without meaning?

**Common violations:**
- Too many competing calls to action at the same visual weight
- Promotional or marketing content mixed into functional UI
- Overly complex data tables showing columns the user rarely needs
- Dense text blocks where progressive disclosure would be better
- Decorative elements that compete with functional content
- Too many font sizes, colours, or weights creating visual noise

---

## H9 — Help Users Recognise, Diagnose, and Recover from Errors

**Definition:** Error messages should be expressed in plain language (no codes), precisely indicate the problem, and constructively suggest a solution.

**What to look for in screenshots:**
- Visible error messages — are they in plain language?
- Error placement — are errors shown near the relevant field or action?
- Error content — do they explain what went wrong AND what to do next?
- Visual treatment — are errors clearly differentiated (typically red, but with icon too for accessibility)?
- Inline validation vs page-level errors

**Note:** Only assessable if an error state is visible in the screenshot.

**Common violations:**
- Error codes or technical messages exposed ("500 Internal Server Error")
- Vague errors that don't explain the cause ("Something went wrong")
- Errors that identify the problem but not the solution ("Invalid input")
- Errors placed far from the relevant field
- Error styling that relies on colour alone (accessibility issue)
- Form errors shown only at top of page without field-level indication

---

## H10 — Help and Documentation

**Definition:** Even though it is better if the system can be used without documentation, it may be necessary to provide help and documentation. Such information should be easy to search, focused on the user's task, list concrete steps to be carried out, and not be too large.

**What to look for in screenshots:**
- Help links, tooltips, or "?" icons
- Contextual help near complex or unfamiliar interactions
- Onboarding or instructional text for first-time use
- Empty state guidance (what to do when there's no content yet)
- Accessible documentation links

**Note:** Often not assessable from a functional screen — more visible on empty states, onboarding screens, or complex forms.

**Common violations:**
- Complex or unfamiliar interactions with no guidance or tooltip
- Empty states that show nothing rather than guiding next steps
- Help only accessible via a distant help centre link, not contextually
- Onboarding skipped entirely for complex features
