# Setup

The has platform has 2 essential parts
- the Unity part (Codename: Droid) 
- the Python part (Codename: Neo)

## Neo

The Neodroid 'Neo' python interface is hosted at PYPI and thus is installable through pip:

```bash
pip3 install -U neodroid
```

Ensure installation was successful, otherwise install missing dependencies. Consult an internet search engine for error messages
If installation was successful, you should now be able run an example environment, directly from your terminal:

```bash
neodroid-mab
```

### neodroid-mab
neodroid-mab is a small demo of Reinforcement Learning experiment
En vindue med tre farvede bokse vil vise sig og blinke løs, hvad man så kigger på er en instans af 
Multi-Armed-Bandit problemmet.

Her er en lærende process prøver at finde og vælge de(n) mest værdifulde boks(e). Hver boks har en chance for at udløse en gevindst af en defineret størrelse, gevindstchancen og gevindststørrelsen er variende fra boks til boks men konstant under afviklingen af forsøget.

Når en boks vælges bliver den enten rød eller grøn, hvor rød betyder at der ikke blev udløst en gevinst (et tabt spil) og grøn betyder at en gevinst blev udløst (et vundet spil).

Over boksende er den faktisk inbyrdes værdi spredning for hver arm (hver boks) og nedenfor er hvad den lærende process tror den inbyrdes forventet værdi spredning er.

En højere inbyrdes værdi betyder at en arm vil være værdifuld at trække i, over tid hvor der taget højde til for hvor sandsynlig en gevindst er og størrelsen af den genvindst (Højere forventet værdi = Mere forventet genvindst)

## Droid
Hent 'droid' (Kodenavn for unity-siden af platformen):

wget https://github.com/sintefneodroid/droid/releases/download/v0.0.3/droid.unitypackage
og importer den til et unity projekt (et eksisterende eller helt nyt, man kan man fordel udnyttet den indbyggede modularitet af de bygget værktøjer til at integere det med eksterende unity-projekter og spil).

