GRADPATH FILES
==============

Files to place in the root of your GitHub repository:
- index.html  (main sign-in tracker; includes Publish my view button)
- view.html   (public read-only viewer with Mihir and Meghana profile tabs)

BEFORE COMMITTING view.html
1. Open view.html in a text editor.
2. Near the bottom, find:
   const SUPABASE_URL = 'PASTE_YOUR_SUPABASE_PROJECT_URL_HERE';
   const SUPABASE_PUBLIC_KEY = 'PASTE_YOUR_SUPABASE_PUBLISHABLE_OR_ANON_KEY_HERE';
3. Replace the placeholders with the project's URL and public publishable/anon key.
   Do NOT use a service_role or secret key. The public key is intended for browser use;
   the SQL policies limit writes to each authenticated owner and the viewer only reads
   rows from gradpath_public_views.
4. Save the file.

UPLOAD
1. Open https://github.com/mihirjayaprakash/gradpath
2. Replace the existing index.html with this index.html.
3. Use Add file > Upload files to add view.html and commit both changes to main.
4. Wait for GitHub Pages to publish.

PUBLISH A PROFILE
1. Open the main tracker and sign in as the relevant account.
2. Click Publish my view.
3. Enter exactly Mihir or Meghana to select the public label.
4. Read the confirmation warning before publishing. Published notes/tasks can be seen by anyone.
5. Open https://mihirjayaprakash.github.io/gradpath/view.html to view the public snapshot.

The read-only viewer is a public snapshot, not a live view of private tables. It changes only when that account publishes again.
