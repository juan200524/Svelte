<script>
  export let pais;
  let p;
  const paises = {
  "colombia":["Colombia", "Bogotá", "51,52 millones", "Peso colombiano", "1, 142 millones km²", "Flag_of_Colombia.svg"],
  "venezuela":["Venezuela", "Caracas", "28,2 millones", "Bolivar"," 916.445 km²", "Flag_of_Venezuela.svg"],
  "ecuador":["Ecuador", "Quito", "17,8 millones", "Dólar estadounidense", "256.370 km²", "Flag_of_Ecuador.svg"],
  "peru":["Peru","Lima","33,72 millones","Sol peruano", "1.285.215 km²", "Flag_of_Peru.svg"],
  "brasil":["Brasil", "Brasilia", "214,3 millones", "Real brasileño", "8,51 millones km²", "Flag_of_Brazil.svg"],
  "argentina": ["Argentina", "Buenos Aires", "45,19 millones", "Peso argentino", "2,78 millones km²", "Flag_of_Argentina.svg"],
  "chile": ["Chile", "Santiago", "19,12 millones", "Peso chileno", "756,1 mil km²", "Flag_of_Chile.svg"],
  "guyana": ["Guyana", "Georgetown", "786 mil", "Dólar guyanés", "214,97 mil km²", "Flag_of_Guyana.svg"],
  "paraguay": ["Paraguay", "Asunción", "7, 13 millones", "Guaraní", "406,75 mil km²", "Flag_of_Paraguay.svg"],
  "surinam": ["Surinam", "Paramaribo", "586 mil", "Dólar surinamés", "63,25 mil km²", "Flag_of_Suriname.svg"],
  "uruguay": ["Uruguay", "Montevideo", "3,47 millones", "Peso uruguayo", "176,22 mil km²", "Flag_of_Uruguay.svg"]

}
p=paises[pais];

</script>

<div class="main">
  <div class="col1">

  </div>
  <img src="./src/assets/{p[5]}" alt="Bandera_Colombia" width="300" height="200">

  <div class="col2">
    <div class="linea"><strong>Pais:</strong> {p[0]}</div>
    <div class="linea"><strong>Capital:</strong> {p[1]}</div>
    <div class="linea"><strong>Población:</strong> {p[2]}</div>
    <div class="linea"><strong>Moneda:</strong> {p[3]}</div>
    <div class="linea"><strong>Extensión:</strong> {p[4]}</div>
  </div>
  
</div>

<style>
  .main {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 5px;
    grid-auto-rows: minmax(100px, auto);
    border-radius: 10px;
    border-style: solid;
    border-color: rgb(185, 190, 182);
    border-width: 2px;
    margin:left;
    width: 650px;
    box-shadow: 5px 5px 5px black;
    margin-right: 5px;
    margin-bottom: 10px;
}

.col1 {
    grid-column: 1;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
}

.col2 {
    grid-column: 2;
    grid-row: 1;
    margin: 5px;
    padding: 5px;
    border-color: black;
    width: max-content;
}
strong {
  color: blue;
  font-weight: bolder;
}
.linea{
  font-size: 20px;
  margin-bottom: 18px;
}
</style>