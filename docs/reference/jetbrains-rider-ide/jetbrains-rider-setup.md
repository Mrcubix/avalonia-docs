---
description: REFERENCE
---

import RiderWelcomeScreenshot from '/img/gitbook-import/assets/jetbrains-rider-setup-1-rider-welcome.png';
import RiderConfigurePluginReposScreenshot from '/img/gitbook-import/assets/jetbrains-rider-setup-2-configure-plugin-repos.png'
import RiderEnterPluginRepoScreenshot from '/img/gitbook-import/assets/jetbrains-rider-setup-3-enter-plugin-repo.png';
import RiderInstallAvaloniaPluginScreenshot from '/img/gitbook-import/assets/jetbrains-rider-setup-4-plugin-install.png';

# JetBrains Rider Setup

To set up _JetBrains Rider_ for developing with _Avalonia UI,_ follow this procedure:&#x20;

- Download and install the .NET SDK of your choice from _Microsoft_. This contains the runtime, development kit (compiler, etc) that is used to build _Avalonia UI_ applications.
- Install the _Avalonia UI_ templates by running the command `dotnet new install Avalonia.Templates` from the command prompt on your machine.

:::info
For the latest .NET SDK downloads, see [here](https://dotnet.microsoft.com/download).
:::

:::info
For SDK versions before .NET 7, you will need to run the command `dotnet new -i Avalonia.Templates`
:::

The output will look similar to this.

```bash
$ dotnet new install Avalonia.Templates
  Determining projects to restore...
  Restored /Users/danwalmsley/.templateengine/dotnetcli/v5.0.200/scratch/restore.csproj (in 706 ms).

Templates                                     Short Name            Language    Tags
.....

Avalonia Resource Dictionary                  avalonia.resource                 ui/xaml/avalonia/avaloniaui
Avalonia Styles                               avalonia.styles                   ui/xaml/avalonia/avaloniaui

Examples:
    dotnet new mvc --auth Individual
    dotnet new mstest
    dotnet new --help
    dotnet new avalonia.mvvm --help
$
```

:::info
To download _JetBrains Rider,_ see [here](https://www.jetbrains.com/rider/).
:::

Rider will give you the very best development experience available for _Avalonia UI_. It is available for Windows, Linux, and macOS. Rider supports XAML out of the box. However, if you want to use the XAML previewer, you will need the Avalonia plugin.

## Install the Avalonia Plugin

Once Rider loads you will see the **Welcome to JetBrains Rider** screen.

- Click **Configure**, and then click **Plugins** on the dropdown menu.

<img src={RiderWelcomeScreenshot} alt="" />

The **Preferences** screen will open.
- Click the settings (gear wheel) icon and then click **Manage Plugin Repositories...** on the popup menu.

<img src={RiderConfigurePluginReposScreenshot} alt="" />

- In the **Custom Plugin Repositories** dialog, click the plus (+) icon and enter the URL `https://plugins.jetbrains.com/plugins/dev/14839`, and then click **OK**.

<img src={RiderEnterPluginRepoScreenshot} alt="" />

- Back at the Preferences window, click **Marketplace** enter 'Avalonia' in the search. Click **AvaloniaRider** when it appears in the search results pane, then click **Install**.

<img src={RiderInstallAvaloniaPluginScreenshot} alt="" />

- After the installation has completed, click **Restart IDE** (button appears).

Now _JetBrains Rider_ is ready to develop _Avalonia UI_ applications.
