<script lang="ts">
</script>

<main>
	<h1>Accounting WEB</h1>
	<table border="solid">
		<thead>
			<th>ID</th>
			<th>DATE</th>
			<th>AMOUNT</th>
			<th>CATEGORY</th>
			<th>TYPE</th>
			<th colspan="2">DESCRIOTION</th>
		</thead>
		<tbody>
			<tr>
				<td data-label="ID">1</td>
				<td data-label="DATE">2021-11-16</td>
				<td data-label="AMOUNT">100</td>
				<td data-label="CATEGORY">Food</td>
				<td data-label="TYPE">UberEat</td>
				<td colspan="2" style="word-break: break-word;" data-label="DESCRIPTION">
					Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
				</td>
			</tr>
			<tr>
				<td data-label="ID">2</td>
				<td data-label="DATE">2021-11-16</td>
				<td data-label="AMOUNT">150</td>
				<td data-label="CATEGORY">Traffic</td>
				<td data-label="TYPE">Uber</td>
				<td colspan="2" style="word-break: break-word;" data-label="DESCRIPTION">
					123456
				</td>
			</tr>
		</tbody>
	</table>
</main>

<style>
	main {
	
		padding: 1em;
		/* max-width: 240px; */
		margin: 0 auto;
	}

	h1 {
		text-align: center;
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 2em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
		h1 {
			font-size: 4em;
		}
	}
	
	table {
  border: 1px solid #ccc;
  border-collapse: collapse;
  margin: 0;
  padding: 0;
  width: 100%;
  table-layout: fixed;
}

table caption {
  font-size: 1.5em;
  margin: .5em 0 .75em;
}

table tr {
  background-color: #f8f8f8;
  border: 1px solid #ddd;
  padding: .35em;
}

table th,
table td {
  padding: .625em;
  text-align: center;
}

table th {
  font-size: .85em;
  letter-spacing: .1em;
  text-transform: uppercase;
}

@media screen and (max-width: 600px) {
  table {
    border: 0;
  }

  table caption {
    font-size: 1.3em;
  }
  
  table thead {
    border: none;
    clip: rect(0 0 0 0);
    height: 1px;
    margin: -1px;
    overflow: hidden;
    padding: 0;
    position: absolute;
    width: 1px;
  }
  
  table tr {
    border-bottom: 3px solid #ddd;
    display: block;
    margin-bottom: .625em;
  }
  
  table td {
    border-bottom: 1px solid #ddd;
    display: block;
    font-size: .8em;
    text-align: right;
  }
  
  table td::before {
    /*
    * aria-label has no advantage, it won't be read inside a table
    content: attr(aria-label);
    */
    content: attr(data-label);
    float: left;
    font-weight: bold;
    text-transform: uppercase;
  }
  
  table td:last-child {
    border-bottom: 0;
  }
}

</style>