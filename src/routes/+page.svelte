<script>
import Button from "../components/Button.svelte";
import Hedding from "../components/Hedding.svelte";
// Až vytvoříš komponent, nezapomeň jej importovat
// Emoji se vytváří pomocí windows + . nebo je můžeš zkopírovat odsud 🙂 😢
</script>

<div class="headings">
    <Heddings heddingTxt={"Svelte"}/>
    <Heddings heddingTxt={"Je"}/>
    <Heddings heddingTxt={"Brnkacka"}/>
</div>

<div class="container">
    <p>Počet: {Pocitani}</p> 
    <div class="buttons">
    <Button></Button>
    </div>
</div>








<style>

    
* {
    font-family: monospace;
}

.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    gap: 10px;
}

.container > p {
    font-size: 2em;
}

.buttons > button{
    border: 1px solid black;
    border-radius: 50000px;
    padding: 10px 20px;
    background-color: lightblue;
    font-size: 1.5em;
}

.buttons > button:nth-of-type(1) {
    background-color: lightblue;
}

.buttons > button:nth-of-type(2) {
    background-color: lightcoral;
}

.headings {
    position: absolute;
}

:global(.headings > h2) {
	position: absolute;
    font-size: 3em;

}

:global(.headings > h2:nth-child(1)) {
	left: 300px;
	top: 50px;
}

:global(.headings > h2:nth-child(2)) {
	left: 200px;
	top: 200px;
}

:global(.headings > h2:nth-child(3)) {
	left: 300px;
	top: 350px;
}


</style>