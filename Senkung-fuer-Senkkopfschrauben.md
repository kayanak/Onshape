# Senkung für Senkkopfschrauben in Onshape erstellen

## Methode 1: Hole Feature (empfohlen)

1. **Sketch erstellen** – Einen Punkt (Center Point) an der gewünschten Position auf der Fläche platzieren
2. **Hole Feature** aufrufen (Toolbar → "Hole")
3. Im Hole-Dialog:
   - **Hole type**: "Counterbore" oder "Countersink" wählen
   - **Standard**: z.B. ISO oder DIN auswählen
   - **Schraubengröße** einstellen (z.B. M5, M6 …)
   - **Countersink angle**: Für DIN-Senkschrauben typischerweise **90°** (DIN 963/965) oder **60°** je nach Norm
   - **Tiefe** festlegen (durch alles = "Through all", oder feste Tiefe)
4. Mit **Grünem Häkchen** bestätigen

## Methode 2: Manuell mit Sketch + Revolve/Chamfer

Falls du mehr Kontrolle brauchst:

1. **Bohrung erstellen** – Sketch → Kreis → Extrude (Remove)
2. **Senkung hinzufügen**:
   - Entweder **Chamfer** auf die obere Kante der Bohrung anwenden
   - Oder einen **Sketch** mit dem Kegelquerschnitt zeichnen und per **Revolve** (Remove) die Senkung erzeugen

## Typische Maße (DIN 7991 – Innensechskant-Senkschraube)

| Schraube | Bohrung ⌀ | Senkkopf ⌀ | Winkel |
|----------|-----------|------------|--------|
| M3       | 3,4 mm    | 6,72 mm   | 90°    |
| M4       | 4,5 mm    | 8,96 mm   | 90°    |
| M5       | 5,5 mm    | 11,2 mm   | 90°    |
| M6       | 6,6 mm    | 13,44 mm  | 90°    |
| M8       | 9,0 mm    | 17,92 mm  | 90°    |

**Tipp:** Das **Hole Feature** ist die sauberste Lösung, da Onshape die Normmaße automatisch hinterlegt und die Bohrung parametrisch bleibt.
