<div class="container">
	<div class="main-area">
		<slot>main area</slot>
	</div>
</div>

<style>
  .container {
    display: grid;
		/* grid-column-gap: 10px; */
		grid-row-gap: 10px;
		grid-template-columns: 1fr 1fr 1fr;
		grid-template-rows: 1fr 1fr 1fr;
		grid-template-areas: 'main main main' 'main main main''main main main'  ;
	}
  .main-area {
		grid-area: main;
		justify-self: stretch;
		align-self: stretch;
	}
</style>
