<div class="main">
	<div class="top-area">
		<slot name="top-slot">top area</slot>
	</div>
	<div class="main-area">
		<slot name="main-slot">main area</slot>
	</div>
	<div class="footer-area">
		<slot name="footer-slot">footer area</slot>
	</div>
</div>

<style>
  .main {
    display: grid;
		/* grid-column-gap: 10px; */
		/* grid-row-gap: 10px; */
		grid-template-columns: 1fr 1fr 1fr;
		grid-template-rows: 0.05fr 1fr 0.2fr;
		grid-template-areas: 'gtop gtop gtop''main main main''footer footer footer'  ;
	}
  .main-area {
		grid-area: main;
		justify-self: stretch;
		align-self: stretch;
	}
	.top-area {
		grid-area: gtop;
		justify-self: stretch;
		align-self: stretch;
	}
	.footer-area {
		grid-area: footer;
		justify-self: stretch;
		align-self: stretch;
	}
</style>
