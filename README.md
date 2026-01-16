# Steps to create HTML Resume

1 - Edit resume.json
    Open resume.json and make the necessary changes.

2 - Validate JSON
    Make sure the JSON is valid and contains no errors.
    Validate via command line:
    python3 -m json.tool resume.json
    Or validate online: https://jsonlint.com/
    
3 - Install resume-cli theme (if not already installed)
    npm install jsonresume-theme-elegant

4 - Regenerate the HTML file
    resume export JulianaPalma_Resume.html --theme elegant
    This generates or updates JulianaPalma_Resume.html based on resume.json.
    Make sure the HTML file is in your project root (or in the folder GitHub Pages serves from, e.g., /docs).

5 - Verify the updated HTML locally
    Open the HTML file in your browser to confirm all changes are correct.

6 - Commit and push the changes
    git add resume.json JulianaPalma_Resume.html
    git commit -m "Update resume JSON and regenerate HTML"
    git push origin main

7 - Configure GitHub Pages (if not already configured)
    Go to your GitHub repo → Settings → Pages
    Under Source, select:
    Branch: main
    Folder: / (root) or /docs if your HTML is in the docs/ folder
    Click Save

8 - Wait for GitHub Pages to update
    Pages may take 30–90 seconds to refresh
    Hard refresh your browser (Cmd + Shift + R on Mac) if needed
    Your updated resume should be visible at:

    https://julpalma.github.io/json-resume/JulianaPalma_Resume.html



