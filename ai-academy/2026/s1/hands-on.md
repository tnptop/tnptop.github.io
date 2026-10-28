# Mini hands-on (1:00-1:15)

15 minutes. Work alone if you have a working Cursor install. Pair with a
neighbor if you do not. This sheet is online at https://tnptop.com/ai-academy/2026/s1/.

## Step 1: Pick one requirement

Pick one of these three. Each is a 3-line requirement, the same shape as
the demo requirement. Each option has an English and a Thai version.
Use either one. The model reads both.

**Option A: Meeting room booking list**
```
We need a simple app to book meeting rooms.
Fields: room name, booked by, date and time.
Add, edit, delete, and view bookings. No login needed.
```

ภาษาไทย:
```
ทำระบบจองห้องประชุมง่าย ๆ ใช้กันภายในทีม
เก็บชื่อห้องประชุม ชื่อคนจอง วัน-เวลาที่จอง
เพิ่ม, แก้ไข, ลบ, ดูตารางจองได้ ไม่ต้องล็อกอิน
```

**Option B: Visitor log**
```
We need a simple log for office visitors.
Fields: visitor name, host employee, check-in time.
Add, edit, delete, and view visitor entries. No login needed.
```

ภาษาไทย:
```
ทำระบบ guestbook ง่าย ๆ สำหรับผู้มาเยี่ยมออฟฟิศ
เก็บชื่อผู้ติดต่อ ชื่อคนที่มาหา เวลาเช็กอิน
เพิ่ม, แก้ไข, ลบ, ดูรายการผู้มาติดต่อได้ ไม่ต้องล็อกอิน
```

**Option C: Team to-do list**
```
We need a simple to-do list for a small team.
Fields: task name, assigned to, due date.
Add, edit, delete, and view tasks. No login needed.
```

ภาษาไทย:
```
ทำ to-do list สำหรับใช้กันเอง
เก็บชื่องาน, คนทำ, deadline
เพิ่ม, แก้ไข, ลบ, ดูรายการงานได้ ไม่ต้องล็อกอิน
```

## Step 2: Ask Cursor for a spec and a plan

1. Use the `ai-academy-demo` folder from the Cursor tour. If it is not
   open, use the **File** menu > **Open Folder**, go to **Documents**,
   select `ai-academy-demo`, and click **Open**. On Windows the button is
   **Select Folder**.
2. Start a new chat: click **+** at the top of the chat panel. Switch it to
   Agent mode. Do not reuse the chat from the tour. A new chat starts with
   an empty context window.
3. Paste your requirement. Below it, in the same message, paste prompt
   (a) from "Prompts from the demo" at the end of this sheet. Then press
   Enter. If you send the requirement alone, Agent builds the whole app
   in one go.
4. Read spec.md. Then send prompt (b). Read plan.md.

## Step 3: Generate and run

1. Send prompt (c). Cursor builds step 1 only.
2. In Files, right-click the generated file and click **Open in Browser**.
   Check step 1.
3. Send prompt (e). Cursor builds the remaining steps.
4. Open the page again and try each action: add, edit, delete, view.
5. If macOS or Windows asks to let Cursor, Chrome, or Python manage other
   apps or accept network connections, click **Don't Allow**. If a
   ManageEngine message says Chrome is blocked, this is company IT
   policy. Close the message. You open the page yourself with
   **Open in Browser**.

If you have time, try prompts (f) and (g).

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

## Prompts from the demo

These are the prompts from the live demo. Copy them, or write your own
in the same shape. Each prompt has an English and a Thai version. Use
either one.

### (a) Spec

```
Before writing any code, turn this requirement into a short spec.
List the data fields, the actions the user can take, and what "done"
looks like for each action. Save it as spec.md.
```

ภาษาไทย:
```
ยังไม่ต้องเขียนโค้ด เอา requirement นี้ไปทำเป็น spec สั้น ๆ ก่อน
บอก field ที่ต้องเก็บ, สิ่งที่ผู้ใช้ทำได้ และแต่ละอย่างทำเสร็จแล้วต้องเป็นยังไง
เซฟเก็บไว้ใน spec.md
```

### (b) Plan

```
Now write a step-by-step plan to build this spec as a single new HTML
file with inline CSS and JavaScript, using localStorage for storage.
Number the steps. Keep each step small enough to check on its own.
Save it as plan.md.
```

ภาษาไทย:
```
เขียน plan ทีละ step ตาม spec เป็นไฟล์ HTML ใหม่ไฟล์เดียว
มี CSS กับ JavaScript อยู่ในไฟล์ เก็บข้อมูลใน localStorage
ใส่เลขทุกขั้น แต่ละขั้นเล็กพอให้เช็กได้ทีละขั้น เซฟเป็น plan.md
```

### (c) Step 1 only

```
Generate step 1 only. Do not write the other steps yet.
```

ภาษาไทย:
```
ทำแค่ step แรกก่อน ขั้นอื่นยังไม่ต้องทำ
```

### (d) Run and check

(d) is not a prompt. Open the page with **Open in Browser** and check
that step 1 does what the plan says.

### (e) The remaining steps

```
Step 1 looks correct. Generate the remaining steps now.
```

ภาษาไทย:
```
ดูดีแล้ว ทำ step เหลือต่อได้เลย
```

### (f) Break it, then fix it

1. In the generated file, rename one function where it is defined.
   Leave every call to it unchanged.
2. Save the file and open the page again.
3. Click the **>_** button at the right end of the browser tab's address
   bar. The developer tools open. Click **Console** and copy the error.

Then send this prompt:

```
I ran this and got this error in the browser console:

<paste the exact console error text here>

Find the cause and fix it.
```

ภาษาไทย:
```
รันแล้วเจอ error นี้ใน console ของเบราว์เซอร์:

<วาง error ตรงนี้>

ช่วยหาสาเหตุแล้วแก้ให้หน่อย
```

### (g) Change the requirement

Type `@` and pick spec.md, so Cursor reads the spec. Send these 3
prompts, one at a time.

```
@spec.md Also record <your change>. Update spec.md only. Do not change the code yet.
```

ภาษาไทย:
```
@spec.md เพิ่ม <สิ่งที่อยากเปลี่ยน> แก้แค่ spec.md ก่อน ยังไม่ต้องแก้โค้ด
```

```
Update plan.md for this change. Show me the plan before you change any code.
```

ภาษาไทย:
```
อัปเดต plan.md สำหรับเรื่องนี้ ขอดูแผนก่อนแก้โค้ด
```

```
The plan looks good. Go ahead.
```

ภาษาไทย:
```
แผนโอเค ลุยเลย
```

Example changes:

- Option A: the end time of each booking.
- Option B: the check-out time of each visitor.
- Option C: a done or not done status for each task.
