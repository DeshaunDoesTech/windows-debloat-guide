# Windows Debloat Guide — No Code Required

### By DeshaunDoesTech

A step-by-step guide to removing unwanted apps, reducing unnecessary startup activity, and cleaning up Windows through its built-in menus.

**No scripts. No terminal commands. No registry edits.** This repository contains documentation only.

[![Buy Me a Coffee](https://img.shields.io/badge/Buy_Me_a_Coffee-Support_DeshaunDoesTech-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=000000)](https://buymeacoffee.com/DeshaunDoesTech)

**[Support my tech content on Buy Me a Coffee](https://buymeacoffee.com/DeshaunDoesTech)**

## Who this guide is for

These instructions focus on **Windows 11** on a personal PC. Menu labels and available switches vary by Windows version, region, and manufacturer. If a setting is missing, use Settings search or skip that optional step.

Windows 10's standard support ended October 14, 2025. Debloating does not extend security support; users staying on Windows 10 should check Microsoft's applicable Extended Security Updates options.

Debloating can reclaim storage and reduce unwanted background activity. It does not guarantee higher gaming FPS, and a low process count is not a useful goal by itself. Removing an app you never run may only save disk space.

## Before you begin

- On a work or school PC, check with your administrator before removing managed applications.
- Back up documents, pictures, saves, and other important files to a separate location.
- Keep account details and installers for paid apps you might reinstall.
- Make a few changes at a time, then test the PC. Keep a note of what you changed.

## Step 1 — Update Windows and record a baseline

1. Open **Start → Settings → Windows Update**.
2. Select **Check for updates**, install applicable updates, and restart if requested.
3. Open **Settings → System → Storage** and note the available space.
4. Right-click **Start → Task Manager**. Observe CPU and memory use after the PC settles.
5. Note any actual problem you want to improve, such as a launcher opening at every sign-in.

Compare results under similar conditions after finishing. Background updates can temporarily affect measurements.

## Step 2 — Create a restore point

1. Open Start and search for **Create a restore point**.
2. Open the result and select the Windows system drive on the **System Protection** tab.
3. If protection is off, select **Configure → Turn on system protection**, assign disk space, and apply the change.
4. Select **Create**, enter a description such as **Before Windows cleanup**, and wait for confirmation.

A restore point is useful for some system changes. It is **not a backup of personal files** and will not recover documents you delete during cleanup.

## Step 3 — Uninstall apps you do not use

1. Open **Settings → Apps → Installed apps**.
2. Review the list; sorting by size can help identify large unused apps.
3. For an app you recognize and no longer need, select its **three-dot menu → Uninstall**.
4. Follow its uninstaller and restart if requested.
5. Repeat with a small group of apps, then test your usual tasks.

Possible candidates include unused promotional games, trial software, duplicate media players, or unused communication and editing apps. Decide by your own usage; there is no universal removal list.

If **Uninstall** is unavailable, leave that component alone in this guide. Do not delete its installation folder manually.

### Keep these unless you have a specific, verified reason

| Component | Why to keep it |
| --- | --- |
| Windows Security, firewall, and security updates | They protect the PC. |
| Microsoft Store and App Installer | Apps may depend on them for installation and updates. |
| Microsoft Edge WebView2 Runtime | Other applications use it to display web-based interfaces. |
| Visual C++ Redistributables and .NET components | Installed programs and games may require particular versions. |
| Graphics, chipset, audio, network, and peripheral drivers | Hardware depends on them. |
| Manufacturer thermal, battery, hotkey, or fan utilities | Some control essential device features. |
| Gaming Services and Xbox-related components you use | Game Pass and certain games may need them. |

Do not remove antivirus software without confirming another supported protection provider is active.

## Step 4 — Reduce startup apps

1. Open **Settings → Apps → Startup**.
2. Turn off optional applications you do not need immediately after signing in.
3. For more context, open **Task Manager → Startup apps** and review startup impact.
4. Restart and check that your normal tasks still work.

Examples might include an unused chat client or a game launcher you prefer to open manually. Keep security tools, required accessibility software, and utilities needed for your hardware.

Turning off startup does not uninstall the app. Open it from Start when needed. To undo this step, turn its startup entry back on.

## Step 5 — Limit optional background activity

1. Open **Settings → Apps → Installed apps**.
2. Open a supported app's **three-dot menu → Advanced options**.
3. If **Background apps permissions** appears, choose **Never** for an app that does not need background updates.
4. Keep **Power optimized** or the appropriate existing setting for apps that need notifications or synchronization.

Some desktop apps do not offer this control. Check their own settings for background operation and launch-at-login options.

An app restricted in the background may stop delivering timely notifications or updates. Restore its previous setting if that happens.

## Step 6 — Tidy Start and the taskbar

1. Open Start, right-click unwanted pinned shortcuts, and choose **Unpin from Start**.
2. Open **Settings → Personalization → Start**.
3. Review the available recommendation and recently added/opened item switches; turn off those you do not want.
4. Open **Settings → Personalization → Taskbar**.
5. Hide optional items, such as Widgets, if you do not use them.

Unpinning and hiding items mainly reduce visual clutter. They do not necessarily uninstall apps or stop all related background processes.

## Step 7 — Reduce notification clutter

1. Open **Settings → System → Notifications**.
2. Review the application list and turn off notifications from unwanted senders.
3. Keep alerts you rely on, especially security and backup notifications.
4. If **Additional settings** appears, review tips, suggestions, and Windows welcome-experience options and disable unwanted prompts.

These choices are about interruptions and personal preference; do not expect a large performance improvement.

## Step 8 — Review temporary files carefully

1. Open **Settings → System → Storage → Temporary files**.
2. Wait for Windows to finish scanning.
3. Read every category before selecting it.
4. Leave **Downloads** unchecked unless you have reviewed and backed up those files.
5. Review the Recycle Bin before emptying it.
6. Select **Remove files** only for the categories you intend to delete.

You can also review **Storage → Cleanup recommendations**.

Deleting a previous Windows installation removes the normal option to go back to that version. Keep it while you are still deciding whether the upgrade works properly. Deleted cleanup files may not be recoverable.

## Step 9 — Configure Storage Sense

1. Open **Settings → System → Storage → Storage Sense**.
2. Enable it only if you want automatic cleanup.
3. Review its schedule and each cleanup rule.
4. Set automatic Downloads cleanup to **Never** if you manage downloads yourself.
5. Choose a Recycle Bin retention period that suits you, or use **Never** and review it manually.
6. Review cloud-content rules before enabling automatic conversion to online-only files.

Online-only cloud files need downloading before offline use. Keep important travel or offline files available locally. Storage Sense primarily manages the Windows system drive; review other drives separately.

## Step 10 — Handle cloud-sync apps separately

Do not uninstall OneDrive or another sync client just because it runs in the background.

1. Decide whether you use its backup or synchronization features.
2. Check that files you need are fully downloaded and open without an internet connection.
3. Make a separate backup of important data.
4. Review the provider's instructions before changing folder backup, unlinking the account, or uninstalling the client.
5. If you are unsure, leave it installed and skip this step.

Deleting files inside a synchronized folder can also delete their cloud copies. Uninstalling a client does not automatically download files that were only stored online.

## Step 11 — Restart and verify

1. Restart the computer.
2. Test internet access, sound, printing, peripherals, and your usual applications.
3. If you game, test your launchers, controller, multiplayer, and Game Pass features.
4. Confirm that Windows Security and Windows Update still function.
5. Compare free storage and startup behavior with your baseline.

Stop once you have removed the clutter that actually bothers you. There is no need to remove every preinstalled app.

## Undoing changes

| Change | How to reverse it |
| --- | --- |
| Uninstalled an app | Reinstall it from Microsoft Store or its official publisher; app data may require your backup. |
| Disabled startup | Re-enable it in Settings → Apps → Startup. |
| Restricted background permissions | Return to Advanced options and restore the previous choice. |
| Hid a taskbar item or disabled notifications | Re-enable it in the same Settings page. |
| Changed Storage Sense | Adjust its rules or switch it off; this does not restore deleted files. |
| System became unstable | Search for Create a restore point → System Restore, choose the earlier point, review affected programs, and follow the wizard. |

If Windows will not start normally, consult Microsoft's recovery instructions linked below. Recovery may require your BitLocker recovery key. Try reversing the most recent change before considering a reset.

## Frequently asked questions

**Will this boost FPS?**  
Possibly in a system constrained by background activity, but there is no guaranteed gain. Storage cleanup and fewer interruptions are more predictable outcomes.

**Should I use a one-click debloater?**  
This guide does not require one. Built-in menus let you review individual changes and avoid bulk removals you do not understand.

**Should I disable Windows services or security features?**  
Not for this guide. Leave the service configuration, Defender protections, firewall, and Windows Update intact.

**Can removed apps come back?**  
An update, reset, reinstall, or manufacturer recovery process can restore some apps or change preferences. Review settings again afterward.

**Why is Windows still using RAM?**  
Windows uses memory for caching and active services. Evaluate responsiveness and memory pressure during real work rather than trying to minimize idle RAM use.

**What if a menu is different?**  
Search within Settings for the feature. If the option is unavailable, skip it instead of forcing a change.

## Quick checklist

- [ ] Back up important files.
- [ ] Update Windows and create a restore point.
- [ ] Remove recognized apps you do not use.
- [ ] Disable optional startup entries.
- [ ] Review supported apps' background permissions.
- [ ] Tidy Start, taskbar, and notifications.
- [ ] Review temporary files before deleting.
- [ ] Configure automatic cleanup deliberately.
- [ ] Restart and test your everyday tasks.

## Official references

Instructions reviewed October 13, 2026. Microsoft may change menu names and feature availability.

- [Microsoft: Uninstall or remove apps and programs](https://support.microsoft.com/en-us/windows/uninstall-or-remove-apps-and-programs-in-windows-4b55f974-2cc6-2d2b-d092-5905080eaf98)
- [Microsoft: Configure startup applications](https://support.microsoft.com/en-au/windows/experience/startup-boot/configure-startup-applications-in-windows)
- [Microsoft: Background apps and privacy](https://support.microsoft.com/en-us/windows/privacy/windows-background-apps-and-your-privacy)
- [Microsoft: System Protection](https://support.microsoft.com/en-us/windows/experience/backup-recovery/system-protection)
- [Microsoft: System Restore](https://support.microsoft.com/en-us/windows/experience/backup-recovery/system-restore)
- [Microsoft: Customize the Start menu](https://support.microsoft.com/en-us/windows/experience/personalization/customize-the-windows-start-menu)
- [Microsoft: Free up drive space](https://support.microsoft.com/en-us/windows/experience/storage-filemanagement/free-up-drive-space-in-windows)
- [Microsoft: Manage drive space with Storage Sense](https://support.microsoft.com/en-us/windows/experience/storage-filemanagement/manage-drive-space-with-storage-sense)
- [Microsoft: Recovery options](https://support.microsoft.com/en-us/windows/experience/backup-recovery/recovery-options-in-windows)
- [Microsoft: Tips to improve PC performance](https://support.microsoft.com/en-us/windows/experience/performance-optimization/tips-to-improve-pc-performance-in-windows)

## Support DeshaunDoesTech

If this guide helped you, consider supporting my tech content and future guides.

**[☕ Buy Me a Coffee](https://buymeacoffee.com/DeshaunDoesTech)**

Support is optional. This guide is free to read.
