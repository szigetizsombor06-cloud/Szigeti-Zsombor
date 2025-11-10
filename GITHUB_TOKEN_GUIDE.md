# How to Create a GitHub Personal Access Token

## Step 1: Create the Token on GitHub

1. Go to GitHub and sign in
2. Click your profile picture (top right) → **Settings**
3. Scroll down to **Developer settings** (left sidebar)
4. Click **Personal access tokens** → **Tokens (classic)**
5. Click **Generate new token** → **Generate new token (classic)**
6. Give it a name (e.g., "Local Development")
7. Set expiration (choose what works for you)
8. Select scopes - **at minimum check:**
   - ✅ **repo** (Full control of private repositories)
9. Click **Generate token**
10. **COPY THE TOKEN IMMEDIATELY** - you won't see it again!

## Step 2: Use the Token to Push

When you run `git push`, it will ask for:
- **Username**: your GitHub username (`szigetizsombor06-cloud`)
- **Password**: paste your Personal Access Token (NOT your GitHub password)

## Alternative: Store Credentials (Optional)

You can configure Git to remember your credentials:
```bash
git config --global credential.helper wincred
```

Then the first time you push, enter your token, and it will be saved.

