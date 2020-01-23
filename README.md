# wp_query
$meta_query_args = array(
	'relation' => 'OR', // Optional, defaults to "AND"
	array(
		'key'     => '_my_custom_key',
		'value'   => 'Value I am looking for',
		'compare' => '='
	),
	array(
		'relation' => 'AND',
		array(
			'key'     => '_my_custom_key_2',
			'value'   => 'Value I am looking for 2',
			'compare' => '='
		),
		array(
			'key'     => '_my_custom_key_3',
			'value'   => 'Value I am looking for 3',
			'compare' => '='
		)
	)
);
$meta_query = new WP_Meta_Query( $meta_query_args );
