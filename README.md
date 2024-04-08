# dotnet_wpf_webview2_example1

```
> dotnet --version
8.0.202
```

[WPF アプリでの WebView2 の概要](https://learn.microsoft.com/ja-jp/microsoft-edge/webview2/get-started/wpf)

```
dotnet new wpf
dotnet add package Microsoft.Web.WebView2
```

```xml
<Window x:Class="dotnet_wpf_webview2_example1.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:dotnet_wpf_webview2_example1"
        xmlns:wv2="clr-namespace:Microsoft.Web.WebView2.Wpf;assembly=Microsoft.Web.WebView2.Wpf"　★★★
        mc:Ignorable="d"
        Title="MainWindow" Height="450" Width="800">
    <Grid>
        <wv2:WebView2 Name="webView"　★★★
                        Source="https://www.microsoft.com"
        />
    </Grid>
</Window>
```