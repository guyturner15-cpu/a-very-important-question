# a-very-important-question

A tiny one-page joke invitation (`index.html`). Everything is in that one file: inline CSS and JS, no build step, no frameworks.

## 1. Get the email working (Web3Forms, free)

1. Go to <https://web3forms.com>, type your email into **Create your Access Key**, and submit.
2. Web3Forms emails you an access key that looks like `a1b2c3d4-....`.
3. Open `index.html`, find this line near the top of the `<script>`, and paste your key in:

   ```js
   const WEB3FORMS_ACCESS_KEY = "YOUR_ACCESS_KEY_HERE";
   ```

The key only lets this page send email **to you**, so it's fine for it to be public. Your email address never appears in the page.

When she taps **go**, the page posts only her time, her food and a UTC timestamp, with the subject `she said yes 💜`. If she goes back and changes her picks, it sends the update. While the key is still the placeholder, nothing is sent and the page shows "screenshot this and send it to me 😌".

Check your spam/promotions folder for the first email.

## 2. Put it online (GitHub Pages)

1. Merge this branch into `main`.
2. On GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, then pick **Branch: `main`** and **folder: `/ (root)`**, and click **Save**.
4. After a minute or two the site is live at <https://guyturner15-cpu.github.io/a-very-important-question/>.

The page sets `noindex` so search engines skip it. The link preview shows "a very important question" / "for stink only".

### Alternative: Netlify Drop

Go to <https://app.netlify.com/drop> and drag in a folder that contains `index.html`. You get a `*.netlify.app` link right away. Create a free account to keep it, because unclaimed drops expire after about an hour.
