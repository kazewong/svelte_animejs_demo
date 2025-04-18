<script>
	import { animate, utils, onScroll } from 'animejs';
	import { onMount } from 'svelte';



	onMount(() => {


	});
</script>

<div class="scroll-container h-screen flex-col content-center">
    <div class="scroll-content flex-col">

        <div class="scroll-section padded h-screen flex justify-center align-middle" id="section1">
            <div class="">	
                <h1 id="title1">Section 1</h1>
            </div>
        </div>

		<div class="scroll-section padded h-screen flex justify-center align-middle" id="section2">
            <div class="">
                <h1 id="title2">Section 2</h1>                
            </div>
        </div>
        
        <div class="scroll-section padded  h-screen" id="section3">
            <div class="flex justify-center align-middle">
                <h1 id="title3">Section 3</h1>                
            </div>
        </div>    
        

    </div>
    
</div>

