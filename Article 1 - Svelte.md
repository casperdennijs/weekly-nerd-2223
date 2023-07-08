# Svelte
Svelte is een nieuw opkomende front-end development framework die gebouwd is om snel webapplicaties mee te kunnen bouwen en te draaien op goede performance. Waarbij andere frameworks zoals React en Vue meer in de browser draait en de virtuele DOM bewerkt, doet Svelte dit bij het opbouwen van de pagina.

Naast Svelte heb je ook SvelteKit van dezelfde makers, dit is een aanvulling die bijvoorbeeld routing makkelijk mogelijk maakt, maar ook in templates te kunnen werken. In Svelte werk je heel erg component gebaseerd wat ervoor zorgt dat je alles heel overzichtelijk en netjes bij kan houden.

In de componenten kan je de HTML, CSS en JS van dat onderdeel verwerken die vervolgens later op een pagina kan oproepen. Dit voorkomt grote lange bestanden die moeilijk leesbaar word en stukken code die op andere pagina's volledig onnodig zijn, maar bijvoorbeeld wel ingeladen worden.

## Voordelen van Svelte
1. **Leerervaring:** Gedurende de Meesterproef heb ik gebruik gemaakt van Svelte en heb ik gemerkt dat het best wel goed te leren is. Er is duidelijke documentatie en veel wordt door Svelte al geregeld. Daarnaast helpt SvelteKit heel erg met het routing van je pagina's en het templaten van je pagina's.

2. **Performance:** De webapp die we hebben gemaakt tijdens de Meesterproef was nog best wel een stukje slordig. Helemaal met code aangezien we voor het eerste keer Svelte(Kit) hebben gebruikt. Ondanks dat alles scoorde we goede cijfers bij Google Lighthouse en loopt de webapp snel. Voor bij kleine webapplicaties is dit goed te merken.

3. **Gebruik:** Svelte is in het begin misschien een beetje uitzoeken, maar dankzij SvelteKit kan je al heel snel aan de gang om websites te maken. Wanneer je hun idee van werken wat meer ontdekt heb kom je er ook achter hoe het makkelijker is.

## Voorbeeld code
```HTML
<script>
  let getal = 0;

  function optellen() {
    getal += 1;
  }
</script>

<main>
  <h1>Svelte Teller</h1>
  <p>Getal: {getal}</p>
  <button on:click={optellen}>Verhoog</button>
</main>

<style>
  main {
    text-align: center;
    padding: 20px;
    font-family: Arial, sans-serif;
  }

  h1 {
    color: #333;
  }

  p {
    color: #666;
    font-size: 18px;
  }

  button {
    padding: 10px 20px;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 4px;
    font-size: 16px;
    cursor: pointer;
  }

  button:hover {
    background-color: #0056b3;
  }
</style>
```
Dit is een eenvoudige Svelte-component die een teller laat zien. De variabele getal wordt gestart met de waarde 0. Wanneer er op de knop "Verhoog" wordt geklikt, moet de functie optellen aangeroepen, die de waarde van getal met 1 verhoogt.

De waarde van getal wordt weergegeven in de paragraaf met behulp van de {getal} tag waarbij de waarde van de getal variabel wordt ingevoegd.

De bijbehorende CSS styling worden uitgeschreven binnen de <style> tags.
