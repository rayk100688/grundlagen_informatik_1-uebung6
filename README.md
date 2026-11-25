# grundlagen_informatik_1-uebung6
tasks for learning the language "Python"
#___________Aufgabe1____________________________
def einmaleins (zahl):
    i=1
    j=1
    print ("  |",end="")
    while i<zahl:
        print (f" {i:2d}|",end="")
        i=i+1
    print (f" {i:2d}|")
    i=1
    print ("--+",end="")
    while i<zahl:
        print (f"---+",end="")
        i=i+1
    print (f"---+")
    i=1
    while i<=zahl:
        print (f"{i:2d}|",end="")
        while j<zahl:
            ergebnis=i*j
            print (f"{ergebnis:3d}|",end="")
            j=j+1
        ergebnis=i*j    
        print (f"{ergebnis:3d}|")    
        i=i+1
        j=1
#Musterlösung enthält eine Variable "zeile" initialisiert mit zeile="" bei jeder Zeilenerzeugung
#Jede spalte macht zeile=zeile+f"{i*j:3d}"
#abschluss mit print(zeile)
#___________Aufgabe2____________________________
def multipledreiecke_v1 (hoehe):
    i=1
    zeile=""
    while i<=hoehe:
        zeile=zeile+f"{i}"
        print (zeile)
        i=i+1
def multipledreiecke_v2 (hoehe):
    i=1
    zeile=""
    while i<=hoehe:
        j=1
        mitte=""
        while j<=(i*2-1):
            mitte=mitte+f"{j}"
            j=j+1
        zeile=" "*(hoehe-i)+mitte+" "*(hoehe-i)
        print (zeile)
        i=i+1
def multipledreiecke_v3 (hoehe):
    i=1
    zeile=""
    while i<=hoehe:
        j=1
        k=1
        mitte1=""
        while j<=i:
            mitte1=mitte1+f"{j}"
            k=j
            j=j+1
        mitte2=""
        j=1
        while k>i-2:
            mitte2=mitte2+f"{j}"
            j=j+1
            k=k-1
        zeile=" "*(hoehe-i)+mitte1+mitte2
        print (zeile)
        i=i+1    
    
