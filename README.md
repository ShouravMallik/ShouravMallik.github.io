How to edit social links and sections

1) Social links (GitHub / Facebook):
- Open `index.html` and find the social icons in the Contact section (look for id `github-link` and `facebook-link`).
- Replace the `href="#"` with your profile URL, for example:
  - `https://github.com/yourusername` or
  - `https://facebook.com/your.profile`
- Alternatively, you can set the links dynamically in the inline script at the bottom of the Contact section. Example:

  document.getElementById('github-link').href = 'https://github.com/yourusername';
  document.getElementById('facebook-link').href = 'https://facebook.com/your.profile';

2) Education entries:
- Open `index.html` and find the section with id `education`.
- Edit the list items inside the `<ul>` to update school/college names, years or add/remove items.

3) Achievements dropdown:
- In the navbar, there is an "Achievements" dropdown. Items have ids `ach-academic` and `ach-cocurricular`.
- To change the displayed text, update the text content inside the `<a>` element.
- To make an item point to a section or page, set its `href` to an anchor (like `#my-achievements`) or a full URL.

Notes
- The contact phone and email are already set in the Contact section. Edit them directly if needed.
- CSS for the social icons is in `style.css` under the `.social-icons` selector.

If you want, I can also make these fields editable from a small JSON file and load them automatically. Let me know if you want that improvement.