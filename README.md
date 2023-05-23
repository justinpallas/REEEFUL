# Rechnergestützter Entwurf eingebetteter Echtzeitsysteme für unbemannte Luftfahrzeuge

## Übung 5 (Positionsbestimmung)

Kombination von GPS und IMU in Matlab
Die Kombination von GPS (Global Positioning System) und IMU (Inertial Measurement Unit) ist eine effektive Methode zur Navigation von Drohnen und anderen autonomen Fluggeräten. Während GPS-Signale eine hochpräzise Positionierung in der horizontalen Ebene ermöglichen, sind sie in der vertikalen Ebene weniger zuverlässig, insbesondere in urbanen Gebieten oder in der Nähe von hohen Gebäuden, wo das GPS-Signal von Gebäuden und anderen Hindernissen blockiert oder reflektiert werden kann. Die IMU hingegen bietet kontinuierliche Messungen von Beschleunigung und Winkelgeschwindigkeit in allen drei Raumrichtungen, was eine genaue Bestimmung der Bewegungen und Ausrichtung der Drohne ermöglicht.

Durch die Kombination von GPS- und IMU-Daten können die Vorteile beider Systeme genutzt und ihre jeweiligen Nachteile ausgeglichen werden. Die Sensorfusion von GPS und IMU verbessert die Positionierungsgenauigkeit und Stabilität der Drohnenflugbahn, was für Anwendungen wie Vermessung, Kartierung, Inspektion und Überwachung von Gebäuden und Infrastruktur, Rettungs- und Notfallmissionen sowie automatisierte Landungen von großer Bedeutung ist.

Im Anhang befindet sich ein Matlab Live-Script (IMUandGPSFusionExample) für Matlab/Simulink. Dieses Skript bestimmt die Position eines Fahrzeugs mithilfe von GPS und IMU. Das ursprüngliche Skript wurde um drei Methoden erweitert: 'ideal', 'fusion' und 'calc'.

Während 'ideal' die Referenzdaten übernimmt und keine Abweichung auftritt, verwendet 'fusion' ein Schätzmodell zur Bestimmung der aktuellen Position abhängig von einer festgelegten Anzahl von Schritten.

Aufgabe 5.1

Erarbeiten Sie sich den Ablauf und die Funktionen des Live-Scripts. Sie können dazu die Hilfefunktion von Matlab nutzen. Fassen Sie den Ablauf und die Funktionalität knapp zusammen und ergänzen Sie diese als Kommentare in Ihrem Live-Script.

Aufgabe 5.2
Implementieren Sie in Ihrer Kopie des Live-Scripts die Methode 'calc'. Diese Methode soll ähnlich der Methode 'fusion' Ihre aktuelle Position unter Verwendung der einzelnen Sensordaten berechnen/schätzen. Vergleichen Sie dazu Ihre Position mit der exakten Position über die Funktion 'ideal'.
Aufgabe 5.3
Erweitern Sie das Modell um einen Drucksensor und schätzen Sie die Höhe des Fahrzeugs durch eine Kombination aller Sensoren und Berechnungen mittels der barometrischen Höhenformel aus der Vorlesung.

Aufgabe 5.4
Geben Sie das vollständige Live-Script kommentiert ab. Benennen Sie das Archiv "NameVorname".
