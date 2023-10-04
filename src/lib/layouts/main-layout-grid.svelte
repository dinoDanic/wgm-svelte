<script>
	let grid = {
		class:
			'grid h-[100vh] relative grid-cols-[minmax(1fr,_1fr)_4fr] grid-rows-[55px_1fr_auto] gap-xs p-xs md:grid-cols-[minmax(250px,_250px)_4fr]'
	};
	let left = {
		class: 'row-span-2 p-xs rounded-md bg-background-sidebar hidden md:block'
	};
	let bar = {
		class: 'col-span-3 md:col-span-2'
	};
	let content = {
		class: 'max-w-full overflow-hidden col-span-3 md:col-span-2 lg:col-span-1 sticky top-0'
	};
	let bottom = {
		class: 'w-full md:w-auto md:bottom-auto md:relative col-span-3'
	};
</script>

<div {...grid}>
	<div {...left}>left</div>
	<div {...bar}>bar</div>
	<div {...content}><slot /></div>
	<div {...bottom}>bottom</div>
</div>
