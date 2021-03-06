---
title: Troubleshooting
order: 4
---

{% include h title="Updating" %}

Normally, the plugin update should go seamlessly. In case of any issues,
 try refreshing the project (click **Refresh** in the Cargo tool window) or rebuilding indices (
**File | Invalidate caches / Restart** from the main menu).
 
Previous versions of the plugin are available at the
[JetBrains plugin repo](https://plugins.jetbrains.com/plugin/8182).


{% include h title="Toolchain setup" %}

To make sure your toolchain is set up correctly, 
go to `Settings / Preferences | Languages & Frameworks | Rust` and check the `Toolchain location` 
and `Standard library` paths.


{% include h title="Cargo project structure" %}

*Currently, the plugin supports only the Cargo-based Rust projects.*

Check the Cargo tool window to make sure your project is imported properly. To force the project structure update, click **Refresh** in the Cargo tool window 
(or call **Refresh Cargo project** using `Help | Find Action`).
 You should see a notification about the successful update.


{% include h title="Macro expansion" %}

If your code includes macros or you experience problems with name resolve, highlighting, or some analysis features (especially related to methods of primitive types),
 try switching to the experimental macro expansion engine in `Settings / Preferences | Languages & Frameworks | Rust`, 
 **Expand declarative macros**. 


{% include h title="Filing a bug" %}

If neither of these tips help, feel free to file an [issue] 
(use the `Help | Create New Issue` action to quickly fill the form in) or ping us in [gitter].


[issue]: https://github.com/intellij-rust/intellij-rust/issues
[gitter]: https://gitter.im/intellij-rust/intellij-rust
