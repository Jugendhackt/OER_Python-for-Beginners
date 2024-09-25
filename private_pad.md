

# Ablauf


  Ablauf Python Workshop:

* Abschnitt 1: Willkommen(30 min)
    * Teilnehmende ankommen lassen und ggf. Eltern verabschieden
    * Teilnehmenden Covid Tests anbieten
    * Namensschilder verteilen
    * Laptops verteilen
    * Willkommen
      * Kurzes willkommensspiel (Massive Multiplayer Schnick Schnack Schnuck)
      * Vorstellen
        * Habt ihr schonmal programmiert?
        * Was wollt ihr heute lernen wie ist euer Wissensstand?
        * Was interessiert euch am meisten?
        * Was ist programmieren eigentlich?
* Abschnitt 2: Präsentation (15 min)
    * Ablauf vorstellen
    * Pad zeigen (https://pad.alpaka.space/[meinlabname])
    * Pause (15 min)
* Abschnitt 3: Code Along (75 min)
    * Into Python
    * Praxisphase
      * Passwörter verteilen
      * Jupyter Notebook aufmachen, einloggen
      * Code Along
    * Pause (15 min)
* Abschnitt 4: Projekte (150 min)
     * Projekt aussuchen
     * Projekt bearbeiten
     * Projekte vorstellen (Stand, was muss noch gemacht werden)
     * Wo finde ich Hilfe wenn ich Fragen habe beantworten?
     * Wie gehts euch / Mood Alpakas klicken https://mood.alpaka.space/berlinlab-feb23
     * Abschied




  # Code-along content

  1. **Hallo Welt!**
      ```python
      print('Hallo Welt!')
      print('Hallo Welt')
      print() #Leerzeile
      print('Mein Name ist NAME')
      ```
      
  2. **Variablen**
      ```python
      mein_name = "$NAME"
      mein_alter = 18
      mein_pi = 3.14
      ```
      Kombiniert:
      ```python
      print("Hallo, ich heiße ", mein_name)
      print(mein_alter)
      print(2 * mein_alter)
      ```
      
  3. **Kommentare**
      ```python
      # Ich bin ein Kommentar
      # Was im Kommentar steht wird nicht ausgeführt:
      # meinName = "Angela Merkel"
      
      print(mein_name) # Ich bin ein inline Kommentar
      ```
      
  4. **Datentypen**
      ```python
      print(type(mein_name))
      print(type(mein_alter))
      print(type(mein_pi))
      
      mein_bool = 1 > 2
      print(type(mein_bool))
      ```
      Mischen von Datentypen:
      ```python
      ergebnis0 = mein_alter + mein_alter
      print(ergebnis0)
      ```
      
      ```python
      # fails with unsupported operand type(s) for +: 'int' and 'str'
      ergebnis1 = mein_alter + mein_name
      ```
      
      ```python
      ergebnis2 = mein_alter + mein_pi
      print(ergebnis2)
      print(type(ergebnis2))
      ```
      
      
      
  5. **Operatoren**

      ```python
      print( 5 + 999 )
      print( 100 - 50 )
      print( 1 - 5 )
      print( 2 * 3 - 4 )
      ```
      
  6. **Listen**
     
      ```python
      eine_liste = [1,2,3,4]
      print(eine_liste)
      
      noch_eine_liste = ["Hallo", "Test", "String"]
      print(noch_eine_liste)
      
      gemischte_datentypen = ["Hallo", 1, mein_pi, True]
      print(gemischte_datentypen)
      
      print(len(gemischte_datentypen))
      
      print(type(gemischte_datentypen))
      
      print(gemischte_datentypen[0])
      print(gemischte_datentypen[3])
      ```
      
  7. **Boolean operators**
      ```python
      alter_nachbar = 18
      print(mein_alter > alter_nachbar)
      print(mein_alter < alter_nachbar)
      print(mein_alter == alter_nachbar)
      ```
      
      ```python
      # fails with: > not supported between instances of 'str' and 'int'
      print(mein_alter > mein_name)
      ```
      
      
      
  8. **If / else**
      
      ```python
      if mein_alter < alter_nachbar:
          print("Anna ist älter als ich")
      else:
          print("Ich bin älter als Anna")
      
      
      
      wochentag = "Samstag"
      
      if wochentag == "Freitag":
          print("Juhu, endlich Freitag :)")
      else:
          print("Leider kein Freitag")
      ```
      
  9. **For-Schleife**
      ```python
      früchte = ["Apfel", "Kirsche", "Birne", "Apfel", "Pfirsich", "Kiwi"]
      
      for frucht in früchte:
          print(frucht)
      
      # mit range():
      for i in range(0,6):
          print(i , früchte[i])
      
      # Mit if-verknüpft:
      for frucht in früchte:
          if frucht == "Pfirsich":
              print("Der Pfirsich wurde gefunden")
          print(frucht)
      ```
      
  10. **While-Schleife**
      ```python
      i = 1
      while i < 6:
          print(i)
          i += 1
      ```
      Frage an die Teilnehmis: wie sieht die For-schleife mit äquivalentem Output aus?
      ```python
      for i in range(1,6):
          print(i)
      ```
      
  11. **(optional) String operatoren**
      
      ```python
      meinString = "Hallo, mein Name ist Johan"
      print(len(meinString))
      print(meinString.upper())
      print(meinString.lower())
      ```
      
  12. **Funktionen**
      ```python
      def myFunc(var1, var2):
          result = var1 + var2
          return result
      
      print(myFunc(1,2))
      ```

