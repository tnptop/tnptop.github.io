# Mini hands-on (1:00-1:15)

15 minutes. Work alone if you have a working Cursor install. Pair with a
neighbor if you do not. This sheet is online at https://tnptop.com/ai-academy/2026/s1/.

## Step 1: Pick one requirement

Pick one of these three. Each is a 3-line requirement, the same shape as
the demo requirement. Write it in Thai or English. The model reads both.

**Option A: Meeting room booking list**
```
We need a simple list to book meeting rooms.
Fields: room name, booked by, date and time.
Add, edit, delete, and view bookings. No login needed.
```

**Option B: Visitor log**
```
We need a simple log for office visitors.
Fields: visitor name, host employee, check-in time.
Add, edit, delete, and view visitor entries. No login needed.
```

**Option C: Team to-do list**
```
We need a simple to-do list for a small team.
Fields: task name, assigned to, due date.
Add, edit, delete, and view tasks. No login needed.
```

## Step 2: Ask Cursor for a plan

1. Create a new empty folder named `hands-on`. Use the same steps as
   setup Step 4: in the Agents window, click **Start from scratch**, then
   **New Folder**. Then click **IDE**.
2. Open the chat and switch it to Agent mode.
3. Paste your chosen requirement.
4. Ask: "Turn this into a short spec, then a step-by-step plan for a
   single HTML file with inline CSS and JavaScript, using localStorage."

## Step 3: Generate and run

1. Ask Cursor to generate the plan, one step at a time if you have time,
   or all at once if you are short on time.
2. Open the generated file in your browser by double-clicking it.
3. Try each action: add, edit, delete, view.

Your page will look different from your neighbor's page, even with the
same option. The model writes new code each time (topic 7). Check that
each action works. The look does not need to match.

## Reflection questions

Answer these in your own words. They map to the concept map on the
slides (topic 21).

1. Where did the plan differ from what you expected the model to build?
   (cluster 4, spec-driven workflow — the spec and plan are not the same
   as the final code)
2. What did Cursor decide on its own that your requirement did not say?
   For example the date format, or what happens on delete. (cluster 3,
   context engineering — "the model only knows what you show it", and it
   fills every gap you leave)
3. If something did not work when you ran it, what did you do next?
   (cluster 5, verification loop — run, error, feed back)
