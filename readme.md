# CurrencyApps
Aplikasi ini mencakup fungsi penghitungan nilai tukar mata uang dari DOLLAR ke RUPIAH. $1 DOLLAR dianggap senilai Rp. 15.000

# Scope & Functionalities

* User dapat memasukkan angka
* User dapat menyentuh tombol hitung
* User mendapatkan info "INVALID" jika yang dimasukkan berupa text

# How Does it Works?
Diawali dari method `MainWindow` pada class `MainWindow.xaml.cs` kita mendeklarasikan:

```csharp
public MainWindow()
        {
            InitializeComponent();
            currencyController = new CurrencyController();
        }
```
Logika perhitungan terdapat pada class `CurrencyController.cs` sebagai berikut:
```csharp
     public string usdToIdr(string nominal)
        {
            var nominalDouble = Convert.ToDouble(nominal);
            var result = nominalDouble * 15000;
            return Convert.ToString(result);
        }
```


# Follow ig : @rizko28 
