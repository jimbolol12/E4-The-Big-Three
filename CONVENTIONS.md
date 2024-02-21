# Code conventions

**Gebruik tabs voor indendation**

Dit staat niet ter discussie. Configureer uw editor om tabs te gebruiken in plaats van spaties. Met tabbladen kan iedereen het inspringingsniveau gebruiken dat hij verkiest.

# 

 **Leesbaarheid code**

Zorg dat er wanneer dit de leesbaarheid en flow van de code vebetert gebruik te maken van Controllers en Methodes. Zorg dat mappen van Klassen, Methodes en Controllers goed gescheiden wordt. Het project moet duidelijk genoeg zijn zodat een set nieuwe programeurs het op kan pakken en er aan kan verder werken. 

#

**Maak gebruik van Pages**

Dit staat niet ter discussie. Zorg dat wanneer en een nieuwe pagina gemaakt moet worden dit een Page is.

#

**Variabele namen zijn geschreven in lowerCamelCase**

*Voorbeeld van een goede manier om dit te doen:*
```C#
var productWindow
```
*Voorbeeld van een foute manier om dit te doen:*
```C#
var ProductWindow
```

# 

**Variabele namen**

Variabele hebben logische namen die passen bij de functie

*Voorbeeld van een goede manier om dit te doen:*
```C#
var productWindow = new ProductenWindow();
```

*Voorbeeld van een foute manier om dit te doen:*
```C#
var window = new ProductenWindow();
```
dit is dubieus, omdat het gaat om een window, maar het wordt niet gespecificeerd welke window dit it. Als je maar een window gebruikt kan dit een gepaste variabele naam zijn, maar bij meerdere windows is dit geen goede variabele naam.

*Voorbeeld van een foute manier om dit te doen:*
```C#
var gingerbread = new ProductenWindow();
```
#

 **Naamgeving van Klassen en Modules**
   
   Gebruik de naamgeving die overeenkomt met de bedrijfscontext, bijvoorbeeld, als er klassen of modules zijn die betrekking hebben op klantgegevens, noem ze dan Customer of CustomerService.

   *Voorbeeld van een goede manier om dit te doen:*
   ```C#
  public class User
  {
    public string Username { get; set; }

    public string Password { get; set; }  
  }
  ```

  *Voorbeeld van een foute manier om dit te doen:*
   ```C#
  public class User
  {
    public string Price { get; set; }
    
    public string Dimensions { get; set; }  
  }
  ```
  #

  **Opmaak XAML code**
  
  klik in je XAML code op edit/advanced/format document om een nette XAML layout te krijgen.
  #

 **Commentaar en Tekst**
  
  Schrijf commentaren in het Nederlands.

  *Voorbeeld van een goede manier om dit te doen:*
   ```XML
  <!-- Bovenste twee blokken -->

  <Grid Grid.Row="2">
    <Grid.ColumnDefinitions>
        <ColumnDefinition Width="*" />
        <ColumnDefinition Width="*" />
    </Grid.ColumnDefinitions>
  ```
  *Voorbeeld van een foute manier om dit te doen:*
   ```XML
  <!-- blok -->

  <Grid Grid.Row="2">
    <Grid.ColumnDefinitions>
        <ColumnDefinition Width="*" />
        <ColumnDefinition Width="*" />
    </Grid.ColumnDefinitions>
  ```
  Voeg nuttige commentaren toe om complexe delen van de code uit te leggen

  #

 **Code Review:**
  
  Voer regelmatig code-reviews uit om naleving van code conventions te waarborgen en om potentiële problemen vroegtijdig te identificeren.

  #

 **Foutafhandeling**
  
  Zorg voor goede foutafhandeling, inclusief het afvangen en registreren van uitzonderingen.

  Gebruik duidelijke foutberichten.

  *Voorbeeld van een goede manier om dit te doen:*
   ```C#
  else
  {
    ErrorTextBlock.Text = "Ongeldige inloggegevens";
  }
  ```

  *Voorbeeld van een foute manier om dit te doen:*
   ```C#
  else
  {
    ErrorTextBlock.Text = "ERROR";
  }
  ```

  #


