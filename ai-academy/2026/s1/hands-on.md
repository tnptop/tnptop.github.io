# Mini hands-on (1:00-1:15)

15 minutes. Work alone if you have a working Cursor install. Pair with a
neighbor if you do not. This sheet is online at https://tnptop.com/ai-academy/2026/s1/.

## Step 1: Pick one requirement

Pick one of these three. Each is a 3-line requirement, the same shape as
the demo requirement. Each option has an English and a Thai version.
Use either one. The model reads both.

**Option A: Meeting room booking list**
```
We need a simple list to book meeting rooms.
Fields: room name, booked by, date and time.
Add, edit, delete, and view bookings. No login needed.
```

ภาษาไทย:
```
ทีมเราต้องการรายการง่าย ๆ สำหรับจองห้องประชุม
ข้อมูลที่ต้องเก็บ: ชื่อห้อง, ชื่อผู้จอง, วันและเวลาที่จอง
ต้องเพิ่ม, แก้ไข, ลบ, และดูรายการจองได้ ไม่ต้องมีระบบล็อกอิน
```

**Option B: Visitor log**
```
We need a simple log for office visitors.
Fields: visitor name, host employee, check-in time.
Add, edit, delete, and view visitor entries. No login needed.
```

ภาษาไทย:
```
ทีมเราต้องการสมุดบันทึกง่าย ๆ สำหรับผู้มาติดต่อที่ออฟฟิศ
ข้อมูลที่ต้องเก็บ: ชื่อผู้มาติดต่อ, ชื่อพนักงานที่มาพบ, เวลาเข้า
ต้องเพิ่ม, แก้ไข, ลบ, และดูรายการผู้มาติดต่อได้ ไม่ต้องมีระบบล็อกอิน
```

**Option C: Team to-do list**
```
We need a simple to-do list for a small team.
Fields: task name, assigned to, due date.
Add, edit, delete, and view tasks. No login needed.
```

ภาษาไทย:
```
ทีมเล็ก ๆ ของเราต้องการรายการงานที่ต้องทำแบบง่าย ๆ
ข้อมูลที่ต้องเก็บ: ชื่องาน, ผู้รับผิดชอบ, วันครบกำหนด
ต้องเพิ่ม, แก้ไข, ลบ, และดูรายการงานได้ ไม่ต้องมีระบบล็อกอิน
```

## Step 2: Ask Cursor for a plan

1. Use the `ai-academy-demo` folder from the Cursor tour. If it is not
   open, use the **File** menu > **Open Folder**, go to **Documents**,
   select `ai-academy-demo`, and click **Open**. On Windows the button is
   **Select Folder**.
2. Start a new chat: click **+** at the top of the chat panel. Switch it to
   Agent mode. Do not reuse the chat from the tour. A new chat starts with
   an empty context window.
3. Paste your chosen requirement.
4. Ask: "Turn this into a short spec, then a step-by-step plan for a
   single new HTML file with inline CSS and JavaScript, using localStorage."

## Step 3: Generate and run

1. Ask Cursor to generate the plan, one step at a time if you have time,
   or all at once if you are short on time.
2. Open the generated file in your browser by double-clicking it.
3. Try each action: add, edit, delete, view.

Your page will look different from your neighbor's page, even with the
same option. The model writes new code each time (slide 13,
"Keyword: non-deterministic"). Check that each action works. The look
does not need to match.

## Reflection questions

Answer these in your own words. They map to the concept map on the
slides (slide 30, "Concept map: where each keyword goes next").

1. Where did the plan differ from what you expected the model to build?
   (cluster 4, spec-driven workflow — the spec and plan are not the same
   as the final code)
2. What did Cursor decide on its own that your requirement did not say?
   For example the date format, or what happens on delete. (cluster 3,
   context engineering — "the model only knows what you show it", and it
   fills every gap you leave)
3. If something did not work when you ran it, what did you do next?
   (cluster 5, verification loop — run, error, feed back)
