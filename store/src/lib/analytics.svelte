<script>
	import { page } from "$app/stores";

	$: {
		if (typeof gtag !== "undefined") {
			gtag("config", "G-MCCKQY6TMC", {
				page_title: document.title,
				page_path: $page.url.pathname,
			});
		}
	}
</script>

<svelte:head>
	<script async src="https://www.googletagmanager.com/gtag/js?id=G-MCCKQY6TMC">
	</script>
	<script>
		window.dataLayer = window.dataLayer || [];

		function gtag() {
			dataLayer.push(arguments);
		}

		gtag("js", new Date());
		gtag("config", "G-MCCKQY6TMC");
	</script>
</svelte:head>
