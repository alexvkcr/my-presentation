<script>
    console.log('Hi')
</script>

<div>
    <slot />
</div>

<style>
    div {
        transition: 0.3s;
        
	    text-align: center;
	    color: black;
	   	font-family: 'Niconne', cursive;
	    font-weight: 700;
        text-shadow: 2px 2px 0px #eb452b, 
                  4px 4px 0px #efa032, 
                  6px 6px 0px #46b59b, 
                  8px 8px 0px #017e7f, 
                  10px 10px 0px #052939, 
                  12px 12px 0px #c11a2b, 
                  14px 14px 0px #c11a2b, 
                  16px 16px 0px #c11a2b, 
                  18px 18px 0px #c11a2b;
    }
    div:hover{
        text-shadow: 5px 5px 0px #eb452b, 
                  10px 10px 0px #efa032, 
                  15px 15px 0px #46b59b, 
                  20px 20px 0px #017e7f, 
                  25px 25px 0px #052939, 
                  30px 30px 0px #c11a2b, 
                  35px 35px 0px #c11a2b, 
                  40px 40px 0px #c11a2b, 
                  45px 45px 0px #c11a2b;

    }
</style>