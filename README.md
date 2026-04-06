# 10 Fixes for Safari Not Working on Your Mac

If Safari is not working on your Mac, you're not alone — and you're not stuck. Safari issues are among the most common complaints from Mac users, and they show up in a variety of ways: a page that refuses to load, a browser that crashes the moment you open it, tabs that go blank for no reason, or an error message telling you Safari can't open the page. Sometimes Safari launches but sits there spinning endlessly. Other times it won't even open at all.

The good news is that most Safari problems have straightforward fixes. The causes range from something as simple as a bad internet connection to deeper issues like corrupted cache files, outdated software, or conflicting extensions. Whether you're seeing a specific error message or Safari is just behaving strangely, this guide covers every proven fix.

These solutions apply to macOS Sequoia, Sonoma, Ventura, Monterey, and earlier versions. Start from the top and work your way down — the fixes are ordered from quickest to most involved.

<img width="2439" height="1134" alt="image" src="https://github.com/user-attachments/assets/45acda6e-7c1a-480b-b335-87bc97c0ac69" />

---

## Table of Contents

- [Quick Fix Summary](#quick-fix-summary)
- [Why Is Safari Not Working on Mac?](#why-is-safari-not-working-on-mac)
- [How to Fix Safari Not Working on Mac](#how-to-fix-safari-not-working-on-mac)
  - [1. Check Your Internet Connection](#1-check-your-internet-connection)
  - [2. Reload the Page](#2-reload-the-page)
  - [3. Force Quit and Relaunch Safari](#3-force-quit-and-relaunch-safari)
  - [4. Clear Safari Cache and Website Data](#4-clear-safari-cache-and-website-data)
  - [5. Clear DNS Cache](#5-clear-dns-cache)
  - [6. Disable Safari Extensions](#6-disable-safari-extensions)
  - [7. Disable VPN and Proxy](#7-disable-vpn-and-proxy)
  - [8. Check Firewall Settings](#8-check-firewall-settings)
  - [9. Update macOS and Safari](#9-update-macos-and-safari)
  - [10. Reset Safari](#10-reset-safari)
- [FAQ](#faq)
- [Conclusion](#conclusion)

---

## Quick Fix Summary

| Fix | Brief Description |
| --- | --- |
| 1. Check your internet connection | Verify Wi-Fi is connected and test with another browser |
| 2. Reload the page | Press Command+R or use the address bar reload button |
| 3. Force quit and relaunch Safari | Use Option+Command+Esc to kill Safari and restart it |
| 4. Clear Safari cache and website data | Remove corrupted cache files through Safari settings |
| 5. Clear DNS cache | Flush the DNS resolver cache using Terminal |
| 6. Disable Safari extensions | Turn off all extensions to rule out conflicts |
| 7. Disable VPN and proxy | Disconnect VPN and remove proxy configurations |
| 8. Check Firewall settings | Make sure macOS Firewall isn't blocking Safari connections |
| 9. Update macOS and Safari | Install the latest macOS version to get Safari updates |
| 10. Reset Safari | Delete Safari preference files to restore default settings |

---

## Why Is Safari Not Working on Mac?

Before you start troubleshooting, it helps to understand what can actually cause Safari to stop working. Safari depends on multiple system components — your network stack, DNS resolver, WebKit rendering engine, cached data, and macOS itself. A problem with any one of these can make Safari misbehave.

Here are the most common reasons Safari is not working on your Mac:

- **Internet connection problems** — If your Wi-Fi is disconnected, unstable, or your ISP is experiencing an outage, Safari can't load any pages. You'll typically see a "Safari Can't Open the Page" or "You Are Not Connected to the Internet" message.
- **Outdated Safari or macOS** — Apple patches Safari bugs and WebKit vulnerabilities through macOS updates. Running an outdated version means you're exposed to known issues that have already been fixed. Some websites may also refuse to load on older Safari versions.
- **Corrupted cache or website data** — Safari stores cached files, cookies, and website data to speed up browsing. Over time, this data can become corrupted and cause pages to load incorrectly, display blank screens, or fail entirely.
- **DNS resolution failures** — Your Mac uses DNS to translate domain names into IP addresses. If the DNS cache is stale or your DNS server is unresponsive, Safari will fail to resolve website addresses — even though your internet connection is technically working.
- **Conflicting extensions** — Safari extensions can interfere with page loading, block content unexpectedly, or cause Safari to crash. A single buggy or incompatible extension can break the entire browser.
- **VPN or proxy interference** — VPN software and proxy configurations route your traffic through intermediate servers. If the VPN is misconfigured, the server is down, or the proxy settings are stale, Safari loses its ability to reach websites.
- **macOS system bugs** — Occasionally, a macOS update introduces bugs that affect Safari's performance or stability. These are typically fixed in the next point release, but they can cause significant issues in the meantime.
- **Firewall blocking connections** — The built-in macOS Firewall or third-party firewall software can block Safari's outgoing and incoming connections, preventing pages from loading.

If you already have a hunch about what's wrong, skip directly to that fix. Otherwise, start with the first method and work through them in order.

---

## How to Fix Safari Not Working on Mac

### 1. Check Your Internet Connection

The most obvious cause of Safari not loading pages is a broken internet connection. Before you dive into more complex fixes, rule this out first — it takes thirty seconds.

Look at the **Wi-Fi icon** in your Mac's menu bar. If it shows a disconnected state (no filled bars or an exclamation mark), your Mac isn't connected to the internet. Click the Wi-Fi icon, select your network, and enter your password if prompted. If the icon shows a connected state but Safari still won't load pages, the problem could be with your router or ISP rather than your Mac.

The fastest way to confirm whether the issue is Safari-specific or a general network problem is to open another browser — Chrome, Firefox, or any browser you have installed — and try loading the same website. If other browsers can't load pages either, the problem is your internet connection, not Safari. Try restarting your router by unplugging it for 30 seconds, then plugging it back in. If only Safari is failing while other browsers work fine, move on to the next fix.

> **Tip:** You can also test your connection by opening **Terminal** and running `ping -c 5 google.com`. If you see replies with response times, your internet connection is working and the problem is specific to Safari.

---

### 2. Reload the Page

This sounds almost too simple, but a surprising number of Safari issues come down to a page that didn't finish loading correctly. A momentary network hiccup, a slow server, or a JavaScript error on the page can all leave Safari stuck on a blank or partially loaded screen.

Press **Command+R** to reload the current page. Alternatively, you can click **View** in the menu bar and select **Reload Page**. If a standard reload doesn't fix it, try a hard reload that bypasses the cache by pressing **Command+Shift+R**. This forces Safari to download fresh copies of all page resources instead of serving them from the local cache.

If a specific page consistently fails to load, try typing the URL directly into the address bar instead of clicking a bookmark or link. Bookmarks can contain outdated URLs, and links on other pages can be broken. You can also check whether the website itself is down by visiting a status-checking service like downdetector.com from another browser.

> **Tip:** If Safari displays the error "Safari can't open the page," pay attention to the full error message. It often includes a clue — "because the server unexpectedly dropped the connection" points to a server-side issue, while "because your computer isn't connected to the internet" points to a local network problem.

---

### 3. Force Quit and Relaunch Safari

If Safari is frozen, unresponsive, or stuck in a loading state, a regular close might not be enough. The application could be caught in a hung process that won't terminate on its own. Force quitting kills the Safari process completely and gives you a clean start.

Press **Option+Command+Esc** to open the Force Quit Applications window. Select **Safari** from the list and click **Force Quit**. Confirm the action when prompted. Wait a few seconds, then reopen Safari from the Dock, Launchpad, or Spotlight.

If Safari keeps crashing immediately after you relaunch it, the problem is likely corrupted data rather than a temporary glitch. In that case, try holding the **Shift** key while opening Safari — this prevents Safari from reopening windows and tabs from your previous session, which can sometimes be the source of the crash. If Safari launches successfully with the Shift key held, the crash was caused by a specific webpage from your previous session.

> **Tip:** You can also force quit Safari from **Activity Monitor**. Open **Activity Monitor** from **Applications > Utilities**, find Safari in the process list, select it, and click the **X** button in the toolbar. This is useful if the Force Quit window itself is unresponsive.

---

### 4. Clear Safari Cache and Website Data

Corrupted cache files are one of the most common reasons Safari stops working correctly. Safari caches images, scripts, stylesheets, and other website resources locally to speed up page loads. When these cached files become corrupted — which happens more often than you'd expect — Safari can display blank pages, load pages incorrectly, or refuse to load them at all.

To clear Safari's cache and website data:

1. Open **Safari**.
2. In the menu bar, click **Safari** > **Settings** (or **Preferences** on macOS Monterey and earlier).
3. Go to the **Privacy** tab.
4. Click **Manage Website Data**.
5. Click **Remove All** and confirm.

This removes all stored website data including cookies, cache files, and local storage. You'll be signed out of most websites, so make sure you know your passwords before proceeding.

For a more targeted approach, you can clear just the cache without removing cookies. Go to **Safari** > **Settings** > **Advanced** and check the box next to **Show features for web developers** (labeled **Show Develop menu in menu bar** on older macOS versions). Then go to the **Develop** menu in the menu bar and click **Empty Caches**. This clears cached files without logging you out of websites.

> **Tip:** If Safari can't even open long enough for you to access its settings, you can clear the cache manually by deleting the folder at `~/Library/Caches/com.apple.Safari/`. Open **Finder**, press **Command+Shift+G**, paste the path, and delete the contents of the folder.

*Also read: [How to Clear System Data on Mac]()*

---

### 5. Clear DNS Cache

If Safari says it can't open a page but your internet connection is working fine (other browsers load pages normally), the problem might be your Mac's DNS cache. DNS (Domain Name System) translates human-readable domain names like "apple.com" into IP addresses that your computer can connect to. Your Mac caches these translations locally so it doesn't have to look them up every time. When this cache becomes stale or corrupted, Safari can't resolve website addresses — even though the websites are perfectly available.

To flush your Mac's DNS cache, open **Terminal** (you'll find it in **Applications > Utilities** or by searching in Spotlight) and run the following command:

```
sudo dscacheutil -flushcache; sudo killall -HUP mDNSResponder
```

You'll be prompted to enter your administrator password. Type it in (the characters won't appear on screen) and press **Enter**. The command executes silently — if you don't see an error message, it worked.

This command does two things: `dscacheutil -flushcache` clears the DNS cache, and `killall -HUP mDNSResponder` restarts the mDNS Responder service that handles DNS resolution on macOS. Together, they force your Mac to perform fresh DNS lookups for every website you visit.

After flushing the DNS cache, try loading the problematic page in Safari again. If DNS was the issue, pages should start loading immediately.

> **Tip:** If you frequently experience DNS-related issues, consider switching to a faster, more reliable DNS server. Go to **System Settings** > **Network** > **Wi-Fi** > **Details** > **DNS** (or **System Preferences** > **Network** > **Wi-Fi** > **Advanced** > **DNS** on macOS Monterey and earlier) and add `8.8.8.8` (Google) or `1.1.1.1` (Cloudflare) as your DNS server.

---

### 6. Disable Safari Extensions

Safari extensions add functionality to your browser, but they can also break it. A single buggy, outdated, or incompatible extension can cause Safari to crash, prevent pages from loading, slow down browsing dramatically, or display pages incorrectly. Content blockers, ad blockers, and VPN extensions are among the most common culprits because they actively modify network requests and page content.

To disable all Safari extensions at once:

1. Open **Safari**.
2. Go to **Safari** > **Settings** (or **Preferences** on macOS Monterey and earlier).
3. Click the **Extensions** tab.
4. Uncheck every extension in the left sidebar to disable them all.

Now test Safari by loading a few different websites. If Safari works normally with all extensions disabled, one of your extensions is the culprit. Re-enable them one at a time, testing Safari after each one, until you find the extension that's causing the problem. Once you identify it, either update the extension (check the App Store for updates), remove it, or find an alternative.

If Safari won't open at all and you can't access its settings, you can disable extensions manually by removing their files. Open **Finder**, press **Command+Shift+G**, and go to `~/Library/Safari/Extensions/`. Move the contents of this folder to your Desktop as a backup, then try opening Safari again.

> **Tip:** After a major macOS update, some extensions may not be compatible with the new version of Safari. Check the developer's website or the App Store listing to see if an update is available. If the extension hasn't been updated in over a year, it's likely abandoned and should be removed.

---

### 7. Disable VPN and Proxy

VPN software and proxy configurations are a common cause of Safari failing to load pages. VPNs route your internet traffic through remote servers, and proxies act as intermediaries between your Mac and the websites you visit. If the VPN server is slow, overloaded, or down, Safari will appear to be broken even though your internet connection itself is fine. Similarly, stale or misconfigured proxy settings can block Safari's access to the web entirely.

To disconnect your VPN:

1. Go to **System Settings** > **VPN** (on macOS Ventura and later).
2. Toggle off any active VPN connection.

On macOS Monterey and earlier, go to **System Preferences** > **Network** and select your VPN connection, then click **Disconnect**. If you're using a third-party VPN app (like NordVPN, ExpressVPN, or Mullvad), open the app and disconnect from there — some VPN apps manage their connections outside of macOS's built-in VPN settings.

To check and disable proxy settings:

1. Go to **System Settings** > **Network** > **Wi-Fi** > **Details** > **Proxies** (on macOS Ventura and later).
2. Make sure all proxy options are unchecked: **Web Proxy (HTTP)**, **Secure Web Proxy (HTTPS)**, **SOCKS Proxy**, and **Auto Proxy Discovery**.
3. Click **OK**.

On macOS Monterey and earlier, go to **System Preferences** > **Network** > **Wi-Fi** > **Advanced** > **Proxies** and uncheck all proxy protocols.

After disabling VPN and proxy, try loading a page in Safari. If Safari works, the VPN or proxy was the problem. You can try reconnecting to a different VPN server, updating your VPN software, or contacting your VPN provider's support.

> **Tip:** Some corporate and school networks require proxy settings to access the internet. If you disable your proxy and lose all internet access (not just Safari), re-enable it and contact your network administrator for help.

---

### 8. Check Firewall Settings

Your Mac's built-in Firewall can block Safari's network connections if it's configured too aggressively. While the default Firewall settings shouldn't interfere with Safari, custom configurations or third-party firewall software can prevent Safari from making outgoing connections to web servers.

To check your Firewall settings on macOS Ventura and later:

1. Open **System Settings**.
2. Go to **Network** > **Firewall**.
3. If the Firewall is turned on, click **Options**.
4. Make sure **Block all incoming connections** is **not** checked. This setting blocks virtually all incoming network communication, which can interfere with Safari's ability to load pages that require two-way connections (like video streaming, WebSocket connections, or certain web apps).
5. Check the list of applications. If Safari appears in the list with "Block incoming connections" next to it, change it to **Allow incoming connections**.

On macOS Monterey and earlier, go to **System Preferences** > **Security & Privacy** > **Firewall** > **Firewall Options** and check the same settings.

If you're running third-party firewall software (like Little Snitch, Lulu, or Radio Silence), check its rules to make sure Safari and its helper processes aren't being blocked. These applications give you granular control over outgoing connections, and it's easy to accidentally block a connection that Safari needs.

> **Tip:** If you're unsure whether the Firewall is causing the issue, try temporarily turning it off entirely (**System Settings** > **Network** > **Firewall** > toggle off), testing Safari, and then turning it back on. If Safari works with the Firewall off, you know the Firewall configuration needs adjustment.

---

### 9. Update macOS and Safari

Safari doesn't have a standalone update mechanism — it's updated through macOS system updates. Running an outdated version of macOS means running an outdated version of Safari, complete with unfixed bugs, unpatched security vulnerabilities, and missing compatibility updates. If Safari has been acting up since a particular date, check whether an macOS update was released around that time that you haven't installed yet.

To check for and install updates on macOS Ventura, Sonoma, and Sequoia:

1. Open **System Settings**.
2. Go to **General** > **Software Update**.
3. Your Mac will check for available updates. If an update is available, click **Update Now** or **Upgrade Now**.
4. Follow the on-screen instructions. Your Mac may need to restart to complete the installation.

On macOS Monterey and earlier, go to **System Preferences** > **Software Update** and follow the same process.

Make sure your Mac is connected to power (for laptops) and has a stable internet connection before starting an update. Major macOS updates can take 30 minutes to over an hour depending on your Mac's speed and the size of the update. Point updates (like 14.5 to 14.6) are typically faster but still require a restart.

After the update completes and your Mac restarts, open Safari and test it. macOS updates frequently resolve Safari issues because they include new versions of WebKit, Safari's rendering engine, along with bug fixes and performance improvements.

> **Tip:** Enable automatic updates to keep Safari current without having to check manually. Go to **System Settings** > **General** > **Software Update** > **Automatic Updates** and make sure all toggles are enabled, especially **Install macOS updates**.

*Also read: [How to Update Safari on Mac]()*

---

### 10. Reset Safari

If none of the previous fixes resolved your issue, the nuclear option is to reset Safari entirely by deleting its preference files and data. This restores Safari to its default state — as if it were freshly installed. You'll lose your Safari-specific settings, browsing history, bookmarks, and saved data, so this should be your last resort.

Before proceeding, make sure Safari is completely closed. If it's running, force quit it using **Option+Command+Esc**.

To reset Safari by removing its preference and data files:

1. Open **Finder**.
2. Press **Command+Shift+G** to open the "Go to Folder" dialog.
3. Type `~/Library/Preferences/` and press **Enter**.
4. Find the file named **com.apple.Safari.plist** and move it to the Trash (or to your Desktop as a backup).
5. Press **Command+Shift+G** again.
6. Type `~/Library/Safari/` and press **Enter**.
7. Move the **entire contents** of this folder to the Trash (or to your Desktop as a backup). This folder contains your history, bookmarks, top sites, and other Safari data.

Optionally, also clear these additional Safari-related folders for a more thorough reset:

- `~/Library/Caches/com.apple.Safari/` — cached page data
- `~/Library/Saved Application State/com.apple.Safari.savedState/` — saved window and tab state
- `~/Library/Cookies/` — look for the file **Cookies.binarycookies** and delete it

After deleting these files, restart your Mac. When you open Safari, it will launch with completely default settings — no extensions, no cached data, no custom preferences. If Safari works normally after the reset, the problem was caused by corrupted settings or data files.

If you backed up your files to the Desktop and Safari is working correctly now, you can safely delete those backups. If Safari still isn't working after a full reset, the problem likely lies outside Safari itself — it could be a system-level issue, a network configuration problem, or a macOS bug that requires a full system reinstall.

> **Tip:** Before resetting, export your bookmarks first so you don't lose them permanently. Go to **File** > **Export Bookmarks** in Safari and save the HTML file somewhere safe. You can import it back later via **File** > **Import From** > **Bookmarks HTML File**.

---

## FAQ

### How do I reset Safari to default settings?

Safari doesn't have a built-in "Reset" button like some other browsers. To reset Safari to its factory-default state, you need to manually delete its preference and data files. Quit Safari, then use Finder's **Go to Folder** dialog (**Command+Shift+G**) to navigate to `~/Library/Preferences/` and delete **com.apple.Safari.plist**. Next, go to `~/Library/Safari/` and delete the contents of that folder. Finally, clear `~/Library/Caches/com.apple.Safari/` and `~/Library/Saved Application State/com.apple.Safari.savedState/`. Restart your Mac, and Safari will launch as if it were brand new — default settings, no extensions, no history, and no cached data. Make sure to export your bookmarks before doing this if you want to keep them.

### Why does Safari say "can't establish a secure connection"?

This error means Safari can't verify the SSL/TLS certificate of the website you're trying to visit. It usually appears when the website's security certificate has expired, is misconfigured, or was issued by an untrusted authority. However, the problem can also be on your end. An incorrect system clock can cause certificate validation to fail — go to **System Settings** > **General** > **Date & Time** and make sure **Set date and time automatically** is enabled. Outdated macOS versions may also lack support for newer TLS protocols, which causes secure connection failures on modern websites. Clearing your DNS cache and disabling browser extensions (particularly security-focused ones) can also resolve this error. If only one specific website triggers the error, the problem is almost certainly on the website's side, not yours.

### Is Safari better than Chrome on Mac?

For most Mac users, Safari is the better choice. Safari is deeply integrated into macOS and optimized specifically for Apple hardware, which means it consistently uses less RAM, less CPU, and less energy than Chrome. On MacBooks, this translates to noticeably longer battery life — independent tests routinely show Safari extending battery life by one to two hours compared to Chrome under identical workloads. Safari also offers stronger privacy protections out of the box, including Intelligent Tracking Prevention that blocks cross-site trackers by default. Chrome, on the other hand, offers a larger extension ecosystem, better cross-platform syncing (if you use Chrome on Windows or Android), and generally faster adoption of newer web standards. If you live entirely within the Apple ecosystem and prioritize battery life and privacy, Safari is the stronger browser. If you rely heavily on Chrome-specific extensions or need cross-platform consistency, Chrome may serve you better despite its higher resource consumption.

### Why does Safari keep crashing on my Mac?

Repeated Safari crashes are typically caused by one of four things: a problematic extension, corrupted cache data, insufficient system resources, or a macOS bug. Start by disabling all extensions (**Safari** > **Settings** > **Extensions**) and testing whether the crashes stop. If they do, re-enable extensions one by one to find the culprit. If extensions aren't the issue, clear Safari's cache and website data (**Safari** > **Settings** > **Privacy** > **Manage Website Data** > **Remove All**). Check your Mac's available storage — if your startup disk is nearly full, Safari and other apps will behave unpredictably. Go to **Apple menu** > **About This Mac** > **Storage** (or **System Settings** > **General** > **Storage** on macOS Ventura and later) and free up space if you're below 10-15 GB. Finally, make sure macOS is fully updated, as Apple regularly patches Safari crash bugs in point releases. If Safari continues crashing after all of these steps, a full Safari reset (deleting preference files as described in Fix 10) is your best remaining option.

---

## Conclusion

Safari not working on your Mac is frustrating, but it's almost always fixable. Most issues come down to a handful of common causes — a spotty internet connection, corrupted cache, stale DNS, a misbehaving extension, or outdated software. Working through the fixes above in order will resolve the vast majority of Safari problems without requiring any advanced technical knowledge.

Start with the basics: check your connection, reload the page, and force quit Safari. If those don't work, clear your cache and flush your DNS. Still stuck? Disable extensions, check your VPN and firewall, and make sure macOS is up to date. The full Safari reset in Fix 10 is your last resort, but it's effective when nothing else works.

If Safari still isn't functioning after trying every fix on this list, the issue may be system-level. Consider creating a new macOS user account and testing Safari there — if it works in the new account, the problem is confined to your user profile. As an absolute last step, backing up your data and reinstalling macOS will give you a completely clean slate.
