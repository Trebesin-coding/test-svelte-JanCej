<script>
    
    
    let count = 0
    let {buttontext} = $props()

    function Pocitani(){
    if (buttontext === "🙂"){
        let count += 1
    }else{
        let count -= 1
    }
    
    }
</script>


<button onclick={Pocitani}>klik</button>