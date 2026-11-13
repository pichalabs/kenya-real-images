# Submission checklist

Prepared in this repo:
- [x] Version 1.0.0 in both `plugin.json` files, README and CHANGELOG
- [x] Website, privacy, terms and support pages in `docs/` (GitHub Pages)
- [x] Listing text, starter prompts, countries proposal: `listing.md`
- [x] 5 positive + 3 negative test cases: `test-cases.md`
- [x] Release notes: `release-notes.md`
- [x] Logo: `logo-512.png`, `logo-1024.png`, `logo.svg`
- [x] Plugin ZIP: build with the command below (not committed)

Only you can do:
1. Push the repo and enable GitHub Pages (Settings > Pages > Deploy from branch `main`, folder `/docs`). Check the four URLs in `listing.md` load.
2. OpenAI Platform: create or use the org "PichaLabs", give yourself the Apps Management: Write role.
3. Verify the business identity as **PichaLabs** (needs business registration documents in that exact name).
4. Run the 8 test cases in `test-cases.md` and note the results.
5. Fill the submission form from `listing.md`, upload the ZIP and logo, confirm countries, and click Submit.

Rebuild the ZIP (from the repo root):

```bash
python -c "import zipfile,os;r='plugins/kenya-real-images';z=zipfile.ZipFile('submission/kenya-real-images-1.0.0.zip','w',zipfile.ZIP_DEFLATED);[z.write(os.path.join(d,f),os.path.relpath(os.path.join(d,f),r).replace(os.sep,'/')) for d,_,fs in os.walk(r) for f in fs]"
```
