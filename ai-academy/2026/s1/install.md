# Set up Cursor and run your first Agent prompt

- Checked on: Cursor 3.24.9, macOS 15.8.1 (Apple Silicon), 2026-10-09.
- Checked on: Cursor 3.24.9, Windows 11, 2026-10-09.

Same steps with screenshots: open `setup/walkthrough.html` in your browser.

Time: about 20 minutes. Download 5 minutes, install 2 minutes, account 5
minutes, first prompt 5 minutes.

Do these steps before the session. Class time does not include a full
install. See "If it fails" for the time limit in class.

## What you need

- A Mac or a Windows laptop.
- Your work Google account. This is the account of your work email.
  You sign up to Cursor with it in Step 2.
- About 300 megabytes (MB) of free disk space for the download.
- A stable internet connection and about 20 minutes.

## Step 1: Download and install

1. Open `cursor.com/home` in your browser. Type the full address, with
   `/home`. If you already have a Cursor account, `cursor.com` opens
   `cursor.com/agents` instead of the download page.
2. Click the download button for your system. The browser downloads one
   file.

- macOS: the file name ends in `.dmg`. The file is about 300 MB.
- Windows: the file name is `CursorUserSetup-x64-3.24.9.exe`. The file
  is about 205 MB.

**On macOS:**

3. Open the downloaded file. A window shows the Cursor icon, an arrow,
   and an **Applications** folder.
4. Drag the Cursor icon onto the **Applications** folder. Wait until the
   copy finishes.
5. Open Cursor from your **Applications** folder.
6. If macOS asks to allow notifications from Cursor, choose either
   option. It does not change these steps.

**On Windows:**

3. Open the downloaded file. A window titled "Setup - Cursor (User)"
   opens. It shows the **License Agreement** screen.
4. Select **I accept the agreement**. Click **Next**.
5. Click **Next** on each of the next three screens: "Select
   Destination Location", "Select Start Menu Folder", and "Select
   Additional Tasks". Do not change the settings.
6. On the "Ready to Install" screen, click **Install**. Wait until the
   green bar is full. This takes about 1 minute.
7. On the "Completing the Cursor Setup Wizard" screen, keep **Launch
   Cursor** selected. Click **Finish**. Cursor opens.

### No admin rights

Do not run install commands that ask for admin rights or an elevated
account. If the installer asks for that, stop and ask the instructor.

## Step 2: Create your account

Cursor opens a window with the Cursor logo, the text "The best way to
code with AI", and two buttons: **Log In** and **Sign Up**.

1. Click **Sign Up**. Your browser opens a page titled "Welcome to
   Cursor".

   If you already have a Cursor account, click **Log In** instead and
   sign in with it.

   The browser may show a small window "Sign up to Cursor". Click
   **Continue to sign up**. The browser then shows the page "Welcome to
   Cursor".

2. Click the **Google** button. It is the first button at the top, with
   the letter G.
3. Google asks which account to use. Choose your work account. Do not
   choose a personal account.
4. Follow the steps from Google until the browser says you are signed
   in.

You do not need the fields **First name**, **Last name**, and **Email**.

**On macOS:**

The browser may show a small window "Sign in to Cursor". Click
**Continue to sign in**.

5. If the browser shows extra offers or questions, choose **Maybe
   later**.
6. Go back to the Cursor window.

**On Windows:**

The browser may show a small window "Sign in to Cursor desktop" with
your name and your email. Click **Sign in**.

The window can also read "Sign in to Cursor". Then click **Continue to
sign in**.

5. The browser then shows a page that starts with "All set". Click
   **Return to Cursor**.
6. If the browser shows extra offers or questions, choose **Maybe
   later**.
7. Go back to the Cursor window.

## Step 3: Answer the three setup questions

Cursor asks three questions, one screen each. Pick these answers.

1. Screen "Tell us about your role": click **Software engineer**.
2. Screen "What brings you to Cursor today?": click **Coding**.
3. Screen "Here are a few ways to get started": click **Skip** below the
   three cards.

Cursor shows "Getting things ready" for a few seconds. Then it opens the
**Cursor Agents** window. This is the home window. It has a prompt box in
the middle with the grey text "Plan, Build, / for skills, @ for context".

## Step 4: Create a folder for your first prompt

- macOS: above the prompt box are two small pickers, **Start from
  scratch** and **This Mac**.
- Windows: above the prompt box are two small pickers, **Start from
  scratch** and **This PC**.

1. Click **Start from scratch**. A menu opens.
2. Click **New Folder** at the bottom of the menu. A window opens. You
   name the folder in this window.

**On macOS:**

3. In **Save As**, type `ai-academy-test`.
4. Leave **Where** as it is. It points to your home folder.
5. Click **Create**.

**On Windows:**

The window title is "New Local Git Repo".

3. In **File name**, type `ai-academy-test`.
4. Do not change the location. The window opens in your home folder.
5. Click **Create**.

Check: the picker above the prompt box now reads **ai-academy-test** and
**main**. On the left, under **Repositories**, you see
**ai-academy-test** and the text "No agents yet".

## Step 5: Send your first Agent prompt

1. Click in the prompt box.
2. Type this text:
   `Create a file named hello.html that shows the text Hello from Cursor in large letters.`
3. Press Enter.

### What you see

**On macOS:**

- A chat named "Hello.html file creation" opens. On the right you see
  **Changes**, **Browser**, **Terminal**, and **Files**.
- Cursor shows lines like "Thought briefly", "Edited hello.html", and
  "Verifying the page renders in the browser". This takes 1 to 3
  minutes.
- At the end, Cursor writes "Created hello.html in the project root" and
  shows a card "1 File Changed" with **hello.html**.
- The bottom bar shows **Changes** and **Create Branch & Commit**. You do
  not need to click them.
- The model picker in the prompt box shows **Cursor Grok 4.6 Medium**.
  Leave it. You can change the model later.

**On Windows:**

- A chat named "Hello.html file creation" opens.
- Cursor shows lines like "Thinking", "Exploring", and "Edited
  hello.html". This takes 1 to 3 minutes.
- A panel can open on the right and show a file. You do not need to do
  anything with it.
- At the end, Cursor shows a card "1 File Changed" with **hello.html**.
  The text above the card can differ.
- The bottom bar shows **Changes** and **Create Branch & Commit**. You do
  not need to click them.
- The model picker in the prompt box shows **Cursor Grok 4.6 Medium**.
  Leave it. You can change the model later.

### If Cursor asks before it runs something

If a card appears with the buttons **Skip** and **Run**, read the text in
the card. Click **Run** if the action stays inside your `ai-academy-test`
folder. Click **Skip** if it does not. Cursor writes files inside your
folder without asking. It asks before it writes outside your folder.

**On Windows:**

Windows can show a window titled "Windows Security" during the Agent
run. It asks: "Do you want to allow public and private networks to
access this app?" The app is Python. Cursor starts a small web server
with Python to check the page. Click **Allow**. The Agent then
continues.

### Check the result

**On macOS:**

1. Open Finder.
2. Open your home folder, then the `ai-academy-test` folder.
3. Double-click `hello.html`. Your browser opens it and shows "Hello from
   Cursor" in large letters.

**On Windows:**

1. Open File Explorer.
2. Open your home folder, then the `ai-academy-test` folder. Your home
   folder is `C:\Users\` followed by your user name.
3. Double-click `hello.html`. Your browser opens it and shows "Hello from
   Cursor" in large letters.

If you see that text, your first Agent prompt works.

## Cursor tour check

Session 1 uses the editor window. Open it and find Tab, Ask, and Agent.
You do not need to use them yet. You only need to see that each one is
there.

### Open the editor

1. In the **Cursor Agents** window, click **IDE** at the top right. IDE
   means integrated development environment, the editor.
2. A second window opens. Its title is **ai-academy-test**. The file list
   on the left shows `hello.html`.

### Tab

1. Click `hello.html` in the file list. The file opens.
2. Click at the end of the last line and press Enter.

**On macOS:**

3. Type `<p>Made with ` and wait 2 seconds. Grey text appears after your
   text, for example "Cursor</p>". That grey text is the Tab suggestion.
   Pressing Tab would accept it. Do not press Tab now.
4. Press Escape. Then press Cmd+Z until your typed text is gone.
5. Press Cmd+W to close the file.

**On Windows:**

3. Type `<p>Made with ` and wait 2 seconds. Grey text appears after your
   text, for example `<a href="https://cursor.com">Cursor</a>`. That
   grey text is the Tab suggestion. Pressing Tab would accept it. Do not
   press Tab now.
4. Press Escape. Then press Ctrl+Z until your typed text is gone.
5. Press Ctrl+F4 to close the file.

The file can have a green background and the buttons **Undo** and
**Keep**. They show the changes from the Agent. You do not need to click
them.

### Ask and Agent

1. On the right side of the editor, find the panel named **New Agent**.
   It has a prompt box.
2. Below the prompt box, click the small button with the infinity
   symbol. A list opens: **Agent**, **Plan**, **Debug**, **Multitask**,
   **Ask**. **Agent** has a check mark.
3. Click **Agent** to close the list.

If you saw the grey Tab text and the list with **Agent** and **Ask**,
your install is ready for Session 1.

Shortcut for later:

- macOS: Shift+Cmd+L opens a new Agent in the editor.
- Windows: Ctrl+Shift+L opens a new Agent in the editor.

## If it fails

1. Do not spend more than 10 minutes on your own.
2. Pair with a neighbor who has a working install. Watch the demo on
   their machine.
3. Tell the instructor, so they can look at your laptop at the end of
   the session.

Ask the program lead if you have a question about your account
before the session.
