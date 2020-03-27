PHP - ARRAY
---------------------------------------------
Array sort
---------------------------------------------
$numbers = [1, 4, 8, 12, 16, 20, 30];

usort($numbers, function($first, $second){
	if($first === $second){
		return 0;
	}
	return ($first > $second) ? 1 : -1;
});

var_dump($numbers);
