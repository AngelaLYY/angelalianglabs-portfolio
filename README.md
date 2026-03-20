# Angela Liang Labs — Portfolio

Main landing page for [angelalianglabs.com](https://angelalianglabs.com). Portfolio of apps and games: Random Swap Co-op, Patient Deidentifier, Focus Loop, and more.

## Local preview

```bash
# From this folder
python3 -m http.server 8080
```

Open [http://localhost:8080](http://localhost:8080).

## Deploy to GitHub Pages

1. **From this folder** (the portfolio files are already here), run:
   ```bash
   cd "/Users/angelaliang/Personal AI Projects/angelalianglabs-portfolio"
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/AngelaLYY/angelalianglabs-portfolio.git
   git push -u origin main
   ```

2. If the repo already has content (e.g. you added a README), clone first and copy files in:
   ```bash
   git clone https://github.com/AngelaLYY/angelalianglabs-portfolio.git
   cd angelalianglabs-portfolio
   # Copy index.html, css/, CNAME, README.md from the portfolio folder
   git add .
   git commit -m "Add portfolio site"
   git push origin main
   ```

4. **Enable GitHub Pages**:
   - Repo → **Settings** → **Pages**
   - **Source**: Deploy from a branch
   - **Branch**: `main` / **Folder**: `/ (root)`
   - **Save**

5. **Add custom domain**:
   - In Pages settings, **Custom domain**: `angelalianglabs.com`
   - Click **Save**
   - When DNS is valid, enable **Enforce HTTPS**

## DNS (GoDaddy)

Add these records for `angelalianglabs.com`:

| Type  | Name | Value                |
|-------|------|----------------------|
| A     | @    | 185.199.108.153      |
| A     | @    | 185.199.109.153      |
| A     | @    | 185.199.110.153      |
| A     | @    | 185.199.111.153      |
| CNAME | www  | AngelaLYY.github.io  |

Remove any conflicting A/CNAME records for `@` or `www`.

## Project links

- **Random Swap Co-op**: https://random-swap-game.angelalianglabs.com/
- **Patient Deidentifier**: https://AngelaLYY.github.io/patient-deidentifier/
- **Focus Loop**: Coming soon
