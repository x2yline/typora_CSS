## make tables sortable

> Add these code in the head of html file，make tables in html sortable

```tml
<script type="text/javascript" src="https://code.jquery.com/jquery-1.12.4.js"></script>
<script type="text/javascript" src="https://cdn.datatables.net/1.10.16/js/jquery.dataTables.min.js"></script>
<script type="text/javascript">
	$(document).ready(function() {
    $('table').DataTable( {
        "paging":   false,
        "ordering": true,
        "info":     false,
        "order": [[ 1, "desc" ]]
    } );
} );
</script>
```



Ref: <https://datatables.net/examples/basic_init/zero_configuration.html>