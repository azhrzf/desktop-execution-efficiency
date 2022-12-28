# Halo Bang✌️

__WindowsFormsApp1__: Contoh project WinForm yang menggunakan WPF User Control Library

__WpfControlLibrary1__: WPF User Control Library yang nantinya diimpor di project WinForm

### Caranya
1. Masuk ke file > Add > Existing Project > WpfControlLibrary1.csproj
2. Toolbox > WPF Interoperability > ElementHost
3. ElementHost > Select Hosted Element > WpfControlLibrary1 > UserControl1 > Dock in Parent Container

### Error?
1. UserControl1 tidak keluar: Build, Rebuild, Clean Solution.
2. Missing References, Packages: Listnya di bawah.

### Note
1. Lebih baik masukin __WpfControlLibrary1__ dibawah satu folder yang sama dengan folder project.
2. [Folder jaga-jaga](https://drive.google.com/drive/folders/1uufSwkDyhaXE7_Fgg075Cq4wEhg4ZwZg?usp=sharing) (pilih yang dipakai)

### References
1. DotNetProjects.DataVisualization.Toolkit
1. Microsoft.CSharp
1. PresentationCore
1. PresentationFramework
1. System
1. System.Core
1. System.Data
1. System.Data.DataSetExtensions
1. System.Diagnostics.PerformanceCounter
1. System.Drawing.Common
1. System.Management
1. System.NetHttp
1. System.Reactive
1. System.Reactive.Windows.Forms
1. System.Runtime.CompilerServices.Unsafe
1. System.Threading.Tasks.Extensions
1. System.Windows DAD System.Windows.Forms
1. System.Windows.Forms.DataVisualization
1. System.Windows.Forms.DataVisualization.IN
1. System.Xaml DAD System.Xml
1. System.Xmllinq
1. WindowsBase
1. WindowsFormslntegration 

### Packages (NuGet)
1. DotNetProjects.WpfToolkit.DataVisualization
1. System.Diagnostics.PerformanceCounter
1. System.Drawing.Common
1. System.Reactive
1. System.Reactive.Windows.Forms
1. System.Runtime.CompilerServices.Unsafe
1. System.Threading.Tasks.Extensions
