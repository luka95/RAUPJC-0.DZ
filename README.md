# JMBAG
0036483490
#Pitanje 1.:
Uz prethodnih 6 fileova, tu se sada nalaze i ClassLibrary1.dll i ClassLibrary1.pdb file.
Ako nedostaje neki od .dll fileova, aplikacija se ruši jer on spada u dependency-je te 
aplikacije i ona u tom slučaju nema pristup nekim funkcijama koje su joj potrebene za ispravan rad.
Za ispravan rad aplikacije, poslao bih vam aplikacija.exe i sve pripadajuće .dll ovisnosti (ClassLibrary1.dll).

#Pitanje 2.:
Konzolna aplikacija je koristila staru verziju class library asemblija jer nije napravljen build koji bi
ga zamijenio novim.

#Pitanje 3.:
Ispisalo se "Pero: Hello World".

#Pitanje 4.:
Sadržaj Bin/Debug foldera konzolne aplikacije je ostao nepromijenjen.

#Pitanje 5.:
Ako obrišemo originalni .dll, aplikacija i dalje radi jer se buildanjem .dll automatski 
kopira u Bin/Debug. 

#Pitanje 6.:
U buildanju aplikacije, NuGet provjerava packages.config te skida sve third-party ovisnosti koje nedostaju,
tako da se u packages direktoriju opet nalazi NodaTime direktorij.