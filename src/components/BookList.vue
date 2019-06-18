<template>
	<div>
		<h1>{{title}}</h1>
		<ul>
			<li v-for="book in books">{{book.title}} - {{book.author}}</li>
		</ul>
	</div>
</template>

<script>
	export default {
		name: 'BookList',
		data() {
			return {
				title: 'All Books',
				books: [
					{title: "Lord of the Rings", author: "JRR Tolkien"},
					{title: "Hitchhikers Guide To The Galaxy", author: "Douglas Adams"},
					{title: "Fear & Loathing in Las Vegas", author: "Hunter S. Thompson"}
				]

			}
		}
	}
</script>

<style>
	h1,h2 {
		font-weight: normal;
	}
	ul {
		list-style-type: none;
		padding: 0;
	}
	li {
		display: block;
		margin: 0 10px;
	}
</style>
