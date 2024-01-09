<nav>
	<h1><a href="/">FreeApks</a></h1>
	<ul class="navigation">
		<li class="navlistitem">
			<a class="navlistlink" href="/Games">Games</a>
		</li>
		<li class="navlistitem">
			<a class="navlistlink" href="/Apps">Apps</a>
		</li>
		<li class="navlistitem">
			<a class="navlistlink" href="/Products">Products</a>
		</li>
		<li class="navlistitem">
			<a class="navlistlink" href="/Articles">Articles</a>
		</li>
		<li class="navlistitem">
			<a class="navlistlink" target="_blank" href="https://github.com/WinterSunset95">Contribute</a>
		</li>
	</ul>
	<div class="search">
		<div class="icon">
			<svg width="100%" height="100%" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg">
			<path fill="#000000" d="M505 442.7L405.3 343c-4.5-4.5-10.6-7-17-7H372c27.6-35.3 44-79.7 44-128C416 93.1 322.9 0 208 0S0 93.1 0 208s93.1 208 208 208c48.3 0 92.7-16.4 128-44v16.3c0 6.4 2.5 12.5 7 17l99.7 99.7c9.4 9.4 24.6 9.4 33.9 0l28.3-28.3c9.4-9.4 9.4-24.6.1-34M208 336c-70.7 0-128-57.2-128-128c0-70.7 57.2-128 128-128c70.7 0 128 57.2 128 128c0 70.7-57.2 128-128 128"/>
			</svg>
		</div>
		<input type="text" placeholder="Search" />
	</div>
</nav>

<style>
nav {
	display: grid;
	grid-template-columns: repeat(12, 1fr);
	background-color: var(--secondary);
	box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
	padding: 1rem;
	justify-content: center;
	align-items: center;
}

h1 {
	grid-column: span 12;
	padding: 0;
	margin: 0;
}

h1 > a {
	color: var(--text);
	text-decoration: none;
}

.navigation {
	grid-column: span 12;
	display: flex;
	justify-content: space-between;
	list-style: none;
	margin: 0;
	padding: 1rem 0;
	flex-wrap: wrap;
}

.navlistitem {
	padding: 0.5rem;
}

.navlistlink {
	color: var(--text);
	text-decoration: none;
}

.navlistlink:hover {
	color: var(--highlight);
}

.search {
	grid-column: span 12;
	display: flex;
	align-items: center;
	background-color: var(--text);
	padding: 0.5rem;
	border-radius: 0.5rem;
	border: 1px solid var(--highlight);
}

.search > input {
	border: none;
	background-color: transparent;
	color: var(--highlight);
	font-size: 1rem;
}

.icon {
	width: 2rem;
	height: 2rem;
	margin-right: 0.5rem;
}

@media only screen and (min-width: 768px) {
	h1, .navigation {
		grid-column: span 6;
	}

	.navigation {
		padding: 0;
	}

	.search {
		grid-column: span 12;
	}
}

@media only screen and (min-width: 1024px) {
	h1 {
		grid-column: span 2;
	}

	.search {
		margin-left: 4rem;
	}

	.navigation, .search {
		grid-column: span 5;
	}
}
</style>
