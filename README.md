# ARIN121 Assignment 3: Travel Planner

An AI travel planning assistant built as a system prompt for Google AI Studio Playground. The full prompt is in `system-prompt.md`.

## What the travel planner can do

When you start a conversation without choosing anything specific (for example, "Hi, I need help with a trip"), the planner shows a menu with two activities:

**1. Plan my trip** (from Assignment 2)
- Collects your destination and trip length, plus departure city, dates, travellers, budget, and interests.
- Shows a Trip Summary and asks you to confirm it before building anything.
- Builds a day-by-day itinerary (morning, afternoon, evening) with estimated costs per person and a cost table compared to your budget.
- Ends with a Top tip and three follow-up options.

**2. Help me choose a destination** (new in Assignment 3)
- Asks which places you are considering and what matters most to you (for example beaches, food, or budget).
- Compares the places in a table, says which one it is leaning toward, and asks about your biggest remaining concern.
- Uses your answer to confirm or change its recommendation, then asks if you are ready to choose.
- When you pick a destination, it offers to plan the trip there.

## How to use it

1. In Google AI Studio Playground, paste the contents of `system-prompt.md` into System Instructions.
2. Start a chat. To pick an activity, reply with the menu number (1 or 2), the activity name, or just say what you want in your own words (for example, "Should I go to Lisbon or Barcelona?").
3. You can switch activities at any time, for example "Actually, help me pick between Tokyo and Seoul first." The planner keeps the details you already gave (dates, budget, travellers, interests) so you do not have to repeat them.
4. If you pick a destination in activity 2, say yes when it offers to plan the trip, and it moves to activity 1 with your details carried over.

## Version history

- `main` first commit: Assignment 2 starting prompt, kept unchanged.
- `conversational-features` branch: added the Menu and Activity Selection module and the Destination Chooser activity, then merged into `main` through a pull request.
