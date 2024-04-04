# Tekoäly ja virtuaaliharrastus

## Yleistä

- **Eläinten tuonti:** generoi eläimelle perustiedot
- **Sisällön luonnin avustaminen:** generoi luonne/tarina raakile
- **Kuvien luonti:** mahdollistaa myös harvinaisten tai keksittyjen rotujen kuvittamisen ilman piirustustaitoa
- **Koodausapu**: Auttaa ohjelmointiongelmien ratkaisemisessa
- **Yleinen sparrausapu**: Tarjoaa ideoita ja inspiraatiota


### Vastuullinen tekoälyn käyttö

Kun käytät tekoälyä, muista noudattaa vastuullisuutta:

- Vältä sisällön generointia, joka loukkaa tekijänoikeuksia tai tavaramerkkejä.
- Merkitse selkeästi sisältö, joka on luotu tekoälyavusteisesti.

## Miten päästä alkuun?

### Kuvien luonti

#### Kuvatyökalut, webbiappsit yms.

Alla on lista työkaluista joilla voi luoda kuvia (text-to-image ja/tai image-to-image). Suurinosa näistä on maksullisia, mutta joistakin saattaa löytyä myös ilmainen kokeilu (trial) osuus. Nämä kaikki vaativat internet-yhteyden ja selaimen tai Discordin. Nämä työkalut ovat (enemmän tai vähemmän) sensuroituja, eli välillä syöttämäsi prompti ei välttämättä lähde generoitumaan mikäli tekoäly havaitsee promptissa bannattuja sanoja tai huomaa että generoitu kuva sisältää esim. alastomuutta tai aseita.

Nämä kaikki vaativat palveluun rekisteröitymisen, mutta luottokorttitietoja ne eivät vaadi jos niissä on myös ilmaisia generointeja.

- Midjourney - [https://www.midjourney.com](https://www.midjourney.com) (€10/kk) (toimii myös Discordissa)
- FullJourney - [https://www.fulljourney.ai](https://www.fulljourney.ai) (€10/kk) (toimii Discordissa)
- Limewire - [https://limewire.com](https://limewire.com) (20 ilmaista kuvaa päivässä, muuten €9,99/kk)
- Pika - [https://pika.art/home](https://pika.art/home) (alkuun 250 krediittiä, sen jälkeen päivittäin 30 krediittiä ilmaiseksi, $8/kk) (toimii Discorissa)
- Leonardo AI - [https://leonardo.ai](https://leonardo.ai) (150 tokenia/pv ilmaiseksi, $10/kk)
- Scenario - [https://www.scenario.com/](https://www.scenario.com/) (500 yksikköä/kk ilmaiseksi, $15/kk)
- Bing - [https://www.bing.com/images/create](https://www.bing.com/images/create) (ilmainen)
- Firefly - [https://firefly.adobe.com](https://firefly.adobe.com) (€5,72/kk)
- Nightcafe - [https://creator.nightcafe.studio/](https://creator.nightcafe.studio/) (perusgenerointi ilmaista - 5 krediittiä/kirjautumispäivä, $5.99/kk)
- Copilot - Edge selaimessa (ilmainen)

#### Kuvatyökalut, työpöytäsovellukset

Muutamia työkaluja voi asentaa myös omalle työpöydälleen. Nämä työkalut eivät tarvitse asennuksen jälkeen internet-yhteyttä ja niillä voi luoda kuvia ilman sensurointia, promptaajalla on vain taivas rajana! Nämä työpöytäsovellukset pohjautuvat Stable Diffusion text-to-image malliin ja tätä perusmallia laajentamalla erilaisilla lisäosilla (lora, embeddings, jne) voidaan generoituvaa sisältöä ohjata juuri sellaiseksi kuin haluaa.

Huomaa kuitenkin että nämä sovellukset vaativat koneeltasi runsaasti tehoja (GPU 8GB+ VRAM, mitä enemmän sitä parempi) toimiakseen sujuvasti.

- Automatic1111 - [https://github.com/AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
- ComfyUI - [https://github.com/comfyanonymous/ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- Fooocus - [https://github.com/lllyasviel/Fooocus](https://github.com/lllyasviel/Fooocus)

#### Kuvatyökalut, pilvikoneet

Jos koneesi ei ole tarpeeksi tehokas pyörittämään työpöytäsovelluksia voit käyttää myös pilvilaskentaa apunasi, silloin maksat vain siitä ajasta mitä käytät kuvien generoimiseen. Pilvilaskennan hyödyntämisessä on se etu että saat sensuroimattoman työkalun joka ei kuitenkaan vaadi suuria kustannuksia (vs. tehokas työpöytäkone) ja maksat vain käytöstä (ei kk-pohjaista laskutusta kuten esim. Midjourney/Firefly).

- RunDiffusion - [https://app.rundiffusion.com/login](https://app.rundiffusion.com/login) $1.09/h (medium kone)
- RunPod - [https://app.rundiffusion.com/login](https://app.rundiffusion.com/login) $0.19/h (RTX 3080Ti)

### Ohjaus / Promptaus

Kaikki yllä olevat työkalut perustuvat sanalliseen ohjeeseen joka annetaan tekoälyn suoritettavaksi.Tämä ohje (prompt) on siis sanallinen ilmaisu kuvasta jonka haluat tekoälyn sinulle tuottavan. Riippuen työkalusta, ohje voi olla hyvin lyhyt ja simppeli (Midjourney, Bing, Dall-e) tai se voi olla hyvinkin runsas ja kuvaileva (Stable Diffusion, Leonardo AI, Scenario, jne.). Ohjauksessa kannattaa (ja usein jopa pitää) käyttää englantia, mitä rikkaampaa ja kuvaavampaa kieltä käyttää sitä parempi tulos yleensä on, hyvänä vinkkinä esim. Thesaurus (https://www.thesaurus.com/) kun tarvitsee löytää synonyymeja (vaikka estääkseen värien valumisen “color bleeding” vääriin paikkoihin tai kiertääkseen sensorointia).

**Vinkit ohjaukseen**

- Kirjoita vain mitä haluat nähdä, etenkin jos käyttämäsi työkalu ei sisällä negatiivista ohjausta (negative prompt)
   - Negatiivisieen ohjaukseen kirjoitetaan taas ne mitä et halua nähdä
- Jos kuvailet esineitä tai asioita väreillä, kannattaa käyttää mieluummin synonyymejä kuin väri-sanaa: jos ohjaat “Red car on a garage” saatat huonoimmassa tapauksessa saada punaisen auton punaisessa autotallissa, “Maroon car on a garage” taas tuottaa paljon todennäköisemmin juuri punaisen auton autotallissa. (“color bleeding”)
- Hahmo tai muu kohde näkyy vain osittain kuvassa? Jos hahmosta näkyy vain yläosa voit kokeilla lisätä mm. “full body” termin, mutta vielä varmemmin toimii kun kuvailet millaiset kengät hahmolla on jalassa ja minkä päällä hahmo seisoo: “A female in her 30s is standing on a beach, wearing leather boots with heels, standing on a shore line.”Lisää siis yksityiskohtia sinne mistä ne puuttuu


### Tekstin luonti

#### Tekstityökalut, webbiappsit yms.

- ChatGPT - [https://chat.openai.com/](https://chat.openai.com/)
- Character AI - [https://beta.character.ai/](https://beta.character.ai/)
- Copilot / Bing

#### Tekstityökalut, työpöytäsovellukset

- Oobabooga - [https://github.com/oobabooga/text-generation-webui](https://github.com/oobabooga/text-generation-webui)
- SillyTavern - [https://sillytavernai.com/](https://sillytavernai.com/)








# Markdown Cheat Sheet

## Description
This cheat sheet provides quick access to Markdown syntax commonly used in GitHub `.md` (Markdown) files. It's perfect for beginners and those looking to refresh their memory on Markdown formatting options.

---

## Table of Contents
1. [Text Formatting](#text-formatting)
2. [Lists](#lists)
3. [Additional Resources](#additional-resources)

---

## Text Formatting

### Bold
To make text **bold**, wrap it with two asterisks or underscores.
- `**This is bold text**`
- `__This is also bold text__`

### Italic
To italicize text, wrap it with one asterisk or underscore.
- `*This text is italicized*`
- `_This text is also italicized_`

### Strikethrough
To ~~strikethrough~~ text, wrap it with two tildes.
- `~~This text is struck through~~`

### Underline (Workaround)
GitHub Markdown does not support underlining directly. A workaround is to use HTML:
- `<u>This text is underlined</u>`

### Combining Formatting
You can combine these formatting options:
- `**_This text is bold and italicized_**`
- `~~**This text is bold and struck through**~~`

---

## Lists

### Ordered List
1. First item
2. Second item
3. Third item
   - Indent items to create sublists
     1. Sublist item

Use numbers followed by a period for each item:

```
1. First item
2. Second item
3. Third item
  - Indent items to create sublists
  1. Sublist item
```

### Unordered List
- First item
- Second item
- Third item
  - Indent items to create sublists
    - Nested sublist item
   
Use dashes (`-`), asterisks (`*`), or plus signs (`+`) for each item:

```
- First item
- Second item
- Third item
  - Indent items to create sublists
    - Nested sublist item
```

---

## Additional Resources

- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Markdown Guide](https://www.markdownguide.org/)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

---
