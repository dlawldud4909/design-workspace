<script>
	import anime from 'animejs/lib/anime.es';
	import { onMount } from 'svelte';
	onMount(() => {
		// JS 코드 시작
		// anime({
		// 	targets: '.el1',
		// 	translateX: 500
		// });
		// anime({
		// 	targets: '.el2',
		// 	translateX: 1000
		// });

		// JS 코드 끝
	});
</script>

<!-- HTML 코드 시작 -->
<p>아래 박스는 width, height, background-color, transform을 위한 트랜지션을 결합합니다. 박스 위에 마우스를 올려 속성들의 애니메이션을 보세요.</p>
<div class="box"></div>
<!-- HTML 코드 끝 -->

<style>
	/* CSS 코드 시작 */


	.box {
    border-style: solid;
    border-width: 1px;
    display: block;
    width: 100px;
    height: 100px;
    background-color: #0000FF;
    -webkit-transition:width 2s, height 2s, background-color 2s, -webkit-transform 2s;
    transition:width 2s, height 2s, background-color 2s, transform 2s;
}
.box:hover {
    background-color: #FFCCCC;
    width:200px;
    height:200px;
    -webkit-transform:rotate(180deg);
    transform:rotate(180deg);
}
	/* CSS 코드 끝*/
</style>
