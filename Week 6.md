---
title: Week 6
tags: [CART 310]
created: 2024-02-20T15:24:27.574Z
modified: 2024-02-20T16:49:02.003Z
---

# Week 6

### Design Patterns
- From Christopher Alexander: architecture and urban design studies
	- Set out to contain in books, the best way to do something
	- Trying to codify knowledge everyone knows

- Each page defines a pattern
- A pattern, a solution to a problem in a context, form systems with other patterns
	- emphasizing, that solutions work in *some* contexts, not all
	- Allows one to look at patterns and their problem contexts, ask if it maps to one's problem context
- Common knowledge
	- Needs to be seen multiple times to be evidenced as a pattern

### MECE
Mutually
Exclusive
Collectively
Exhaustive

- Every item should be able to fit into one and only one category,
- Your categories should collectively be able to fit any and all datatypes
- Categorisation scheme needs to be a bit flexible,
- Use card-sorting research!
- if there is something you have to do all the time, make th ecommute as short as possible

## UX Spatial Patterns
### Hub and spoke
- Central starting screen,
- Going back and forth between hub &  other screens
- Makes sense for smaller screens
	- One screen at a time
	- DOes end up requiring backtracking

### Fully connected
- Connections between all screens
- Makes sense for larger screens

### Multilevel/tree
- Some interconnection, but more categorized
- Not as visible in what you could do
- INstead of a constant menu, dropdown menus, to allow people to navigate in between without it being constantly visible

### Pyramid
Similar to hub and spoke, but 

### Step-by-step
- self-explanatory
- Amazon interesting example
	- Different checkout steps used to be separate screens
	- Now different sections all on the same screen

### Card or grid view
- Content of the same type

## Guidance? Missed a slide

### Progress indicator
Seeing all the steps ahead, where you are, etc.

### Breadcrumbs
Seeing categories and subcategories, parents and children
Allows you to go explore other things in similar subcategories

## Flat navigation
- User knows where they are
	- They're not navigating, just trying to figure out what tool to use
	- Manipulating same content
- One wants to think about 

## Atomic design
Instead, of thinking top down, forcing content into existing patterns (pages)
One could think bottom up, what are the smallest elements, atoms
Then grouping these together to think about how atoms work together
Tends to be more consistent

**atoms**
buttons, inputs, labels, icons, etc. - smallest UI element
**molecules**
combining atoms into a meaningful chunk, eg. combine avator atom with name,

Put elements into bigger and bigger boxes

## Input
Nothing natural or obvious about these actions
Patterns that have become standards we now come to expect

### tap, swipe, pinch
- tap
	- select, activate, launch, toggle
- swipe
	- scroll, move between, reveal, hidden action, pan, refresh
- pinch
	- zoom control

### rotate / shake
- rotate
	- change orientation
- shake
	- undo, reset, remix, skip

### Buttons
- placed directly on interface
- grouped semantically (similarity, function)
- Big, readable, easy!
- Take up space

### Menu bars
Standard for most desktop apps
Show a complete set of actions, grouped semantically
Often duplicate functionality also available in context menu and toolbars
	- accessible!

### Toolbars
Like menu bars, but simpler
Row of buttons
Can feature drop down menus and text fields
Icons need to be easily recognizable though

### Tab bars
Very similar to toolbars, but for different screens instead of tools
Again, need recognizable icons

### Navigation drawers
Slides out from left
Menu options
Savevs screen space

### Contextual preview
New content previewed in a floating pane
Only shows for a short amount of time
Incomplete view, moving countdown bar
	- completion vs deletion
	- based on Western languages and reading

### Action panels
Menus that a user doesn't need to open they're just there
Often reliaant on verbal description
more room for words
Actions too complicated for icons,

### Links
Buttons with no borders
OFten understood via coloured underline text
Soem only appear on hover
- obviously can be harder to see, understand as links
Do what you need to do to convey clickability

### Pop-up / contextual menu
Can be difficult to navigate if too long
	- too much text
	- hard to see beginning and end

### hover menu
Always available
But only reminding user in specific contexts
Maintaining balance between readability & functionality

### Splash screenr
Can show you app is loading
Good place to put logo
Can be boring in terms of visual communication

