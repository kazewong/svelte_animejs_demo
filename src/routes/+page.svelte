<script>
	import { animate, onScroll } from 'animejs';
	import { onMount } from 'svelte';

	onMount(() => {
		animate('#title1', {
			x: '15rem',
			rotate: '1turn',
			duration: 2000,
			alternate: true,
			loop: true,
			ease: 'inOutQuad',
			autoplay: onScroll({
				container: '.scroll-container',
				target: '#section1',
				debug: true,
			})
		});
		
		animate('#title2', {
			x: '15rem',
			rotate: '1turn',
			duration: 2000,
			alternate: true,
			loop: false,
			ease: 'inOutQuad',
			autoplay: onScroll({
       			container: '.scroll-container',
       			target: '#title2',
       			debug: true,
			})
		});
	});
</script>

<div class="scroll-container h-screen flex-col content-center">
    <div class="scroll-content f">
        <div class="scroll-section padded" id="section1">
            <div class="flex justify-center align-middle">
                <h1 id="title1">Section 1</h1>
            </div>
        </div>
        
        
        <div class="scroll-section padded" id="section3">
            <div class="flex justify-center align-middle">
                <h1 id="title3">Section 3</h1>                
            </div>
        </div>    
        
        <div class="scroll-section padded" id="section2">
            <div class="flex justify-center align-middle">
                <h1 id="title2">Section 2</h1>                
            </div>
        </div>    
    </div>
    
</div>

