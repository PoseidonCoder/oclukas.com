<script>
	let title = '';
	let letterIndex = 0;
	let fullTitle = "Hi, I'm Lukas";

	const id = setInterval(()=> {
		if (letterIndex >= fullTitle.length) {
			clearInterval(id);
		} else {
			title += fullTitle[letterIndex];
			letterIndex++;
		}
	}, 100)
</script>

<div id="intro" class="section">
    <img id="avatar" alt="me" src="me.png">
    <h1 id="title">
		{title}
		<span id="type">▋</span>
	</h1>
</div>