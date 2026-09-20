# REMINDER / WARNING

> ## CAUTION
> **This information should not be shared anywhere on the internet.**
> You should never let anyone see, nor get information from the DevTools panel, even if it's not suspicious.

You should not trust **ANYONE** with this information. Even your best friends. You don't know when people are going to betray you. Be careful.

> ## I cannot take any responsibility for the damage caused by others.


# ⚠️ THIS INFORMATION IS THE SAME AS A PASSWORD. KEEP IT SAFE. ⚠️

*I used prominent formatting because this is too important to ignore.*

---
<details>

<summary>I have read everything above.</summary>

### How to get this information

1. Go to **https://playvortex.io**

2. Right-click anywhere on the website and click `Inspect`.
   You can also press `F12` or `Ctrl + Shift + I`.

3. Go to `Application`.

4. Find `Cookies`.

5. Select [**`https://playvortex.io`**](https://playvortex.io).

6. Copy the value for `session_token` (I will call it `session_token_value`) and `cf_clearance` (I will call it `cf_clearance_value`).

7. Put them into this text, and you have the full cookie for the API requests:

```text
session_token=[session_token_value]; cf_clearance=[cf_clearance_value]
```

</details>