# Adaptive UI Pattern Library

## Overview
This library contains reusable intelligence patterns that help interfaces adapt to human behavior. Each pattern recognizes when someone is struggling and responds with helpful visual changes.

**Learning Interface Context:**
These patterns are specifically designed to reduce confusion in learning environments by recognizing cognitive load signals and providing contextual visual support. They help learners navigate complex interfaces without overwhelming them, supporting both novice exploration and expert efficiency.

---

## Pattern 1: Focus Assist

**What triggers it:**
- User repeatedly undoes actions (undo-loop behavior)
- Shows confusion or uncertainty about what to do next

**How the UI responds:**
- Highlights the main action button with bright colors
- Makes it larger and more prominent
- Adds a subtle border to draw attention

**Why this helps:**
Reduces cognitive load by eliminating choice paralysis - when learners are confused, highlighting the primary action path helps them progress without mental strain.

**Duration:** 3 seconds

---

## Pattern 2: Hover Relief

**What triggers it:**
- User hovers over the same areas repeatedly (hover-repeat)
- Shows indecision or uncertainty about options

**How the UI responds:**
- Softly fades other tiles with gentle blur
- Highlights the focused area with warm pink glow
- Creates gentle breathing animation to calm anxiety

**Why this helps:**
Supports decision-making by reducing visual noise - when learners show indecision, dimming alternatives helps focus attention and reduces overwhelm.

**Duration:** 4 seconds

---

## Pattern 3: Navigation Guide

**What triggers it:**
- User navigates back and forth between options (backtrack behavior)
- Shows navigation uncertainty or lost feeling

**How the UI responds:**
- Pulses the current area with teal/green colors
- Adds subtle arrow hints on other tiles
- Creates directional visual cues for guidance

**Why this helps:**
Prevents navigation confusion by providing spatial orientation - when learners feel lost, visual cues restore their sense of location and direction.

**Duration:** 3.5 seconds

---

## Pattern 4: Attention Re-centering

**What triggers it:**
- User stays focused on one area for an extended time (dwell behavior)
- Shows deep concentration or careful consideration

**How the UI responds:**
- Gently pulses the focused area with soft animation
- Uses calming blue colors to reinforce attention
- Provides subtle feedback without interruption

**Why this helps:**
Reinforces focused attention without disruption - when learners are deeply engaged, subtle feedback validates their focus and maintains flow state.

**Duration:** 4 seconds

---

## Pattern 5: Quick Combo (Fast Action)

**What triggers it:**
- User performs rapid sequential actions (fast-action behavior)
- Shows confident, experienced interaction patterns

**How the UI responds:**
- Briefly highlights affected areas with quick flash
- Provides immediate visual feedback for rapid interactions
- Uses fast, snappy animations to match user pace

**Why this helps:**
Acknowledges expert behavior by matching interaction speed - when learners demonstrate mastery, responsive feedback maintains their efficient workflow.

**Learning Context Note:**
This pattern is learning-safe as it only activates for confident, rapid actions. It supports advanced learners without overwhelming beginners, since slow, hesitant users won't trigger it.

**Duration:** 1.5 seconds

---

## Implementation Notes

### Pattern Recognition
- Each pattern watches for specific user behaviors
- Behaviors are detected through interaction signals
- Only one pattern can be active at a time to avoid chaos

### Response Timing
- All patterns have automatic timeouts
- Visual changes fade away naturally
- System returns to normal state cleanly

---

## Usage Guidelines

**When to use these patterns:**
- In complex interfaces where users might get lost
- During important decision-making moments
- When user testing shows confusion or hesitation

**When NOT to use:**
- In simple interfaces with obvious actions
- During fast, confident user workflows
- When visual changes might be distracting

**Customization:**
- Adjust timing based on your users' pace
- Modify visual intensity for your brand
- Test with real users to validate effectiveness

---

## Technical Integration

These patterns work with any web interface by:
1. Detecting user behavior signals
2. Mapping signals to appropriate patterns
3. Applying visual responses through CSS classes
4. Automatically cleaning up after timeout

