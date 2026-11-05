# Setup ajmiapps.com (GitHub Pages)

1. impressum.html: replace the two [PLACEHOLDER] lines with your address. Do not publish with the placeholders.
   (Check what you need: legal question, not for me to decide. A P.O. box does NOT replace the required address in most cases.)
2. github.com -> New repository -> name `ajmiapps` (Public). Upload everything from this folder
   (index.html, impressum.html, CNAME, noorradio/ folder). Commit.
3. Repo -> Settings -> Pages -> Source: "Deploy from a branch", Branch `main`, folder `/ (root)` -> Save.
   Under "Custom domain" enter `ajmiapps.com` -> Save. Later tick "Enforce HTTPS".
4. At the domain provider -> DNS settings:
   - 4 x A record, host `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - CNAME, host `www` -> `issameddine2.github.io`
   (Remove any default parking records first.)
5. Wait 10 minutes to a few hours, then open https://ajmiapps.com and https://ajmiapps.com/noorradio/privacy.html
6. Only then change the URLs in App Store Connect (App information -> Privacy Policy URL, version page -> Support URL).
   Keep the old noorradio GitHub page online until the new one works.
