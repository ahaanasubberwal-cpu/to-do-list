Do the following steps in order:

1. **Capture a screenshot** of index.html using Playwright:
   - Run this in the project directory:
     ```
     node -e "const{chromium}=require('playwright');(async()=>{const b=await chromium.launch();const p=await b.newPage({viewport:{width:1280,height:800}});await p.goto('file://'+process.cwd()+'/index.html');await p.waitForTimeout(1000);await p.screenshot({path:'screenshot.png',fullPage:true});await b.close();})()"
     ```

2. **Update README.md** with:
   - Project title and description
   - Screenshot embedded near the top: `![Screenshot](screenshot.png)`
   - Full features list based on what the app actually does
   - Live demo link: `https://ahaanasubberwal-cpu.github.io/to-do-list/`
   - Tech stack section

3. **Push everything to GitHub**:
   - `git add -A`
   - `git commit -m "update readme and screenshot"`
   - `git push origin main`

Report the GitHub repo URL and live site URL when done.
