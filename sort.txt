 <?php
 
 $array = array('52', '-52', '52','-52');
 $max1=0 ; $max2=0;
 for($i=0; $i<count($array); $i++){
 	if($array[$i] > $max1){
 		$max2 = $max1;
 		$max1 = $array[$i];
 	}elseif($array[$i] > $max2){
 		$max2 = $array[$i];
 	}
 
 }
 
 echo $max2;
 die('abid');
 
// outpuut : 52 
 
    $team = "arsenal";
    switch ($team) {
    case "manu":
        echo "I love man u";
        break;
    case "arsenal":
        echo "I love arsenal";
         break;
    case "manc":
        echo "I love manc";
         break;
    case "abc":
        echo "I love abc";
         break;
    
    } 
    
 die;
 
    $total = "25 students";
    $more = 10;
    $total = $total + $more;
    echo "$total";
    // output : 35
    
    function track() {
    static $count = 0;
    $count++;
    echo $count;
    }
    track();
    track();
    track();
    
     // output : 123
     

    
    die;
    ?>
    

<?php

class Animal
{

    public $name = "Hello";

    
    public function __construct($name)

    {

        echo "Live HERE";    

        $this->name = $name;

    }
    
    public function __destruct()

    {

        echo "Destroy here";

    }

}

$animal = new Animal("Bob");

echo "My Name is : " . $animal->name;

die;

$ab= str_replace("interview","interviews","Best interview questions!");

echo $ab; die;

$var = "Best Interview Questions";
ltrim("Best", $var);
rtrim("Questions", $var);
echo $var; die;

$var1 = "This is good interview Question";
echo substr($var1,8);
die;
$mainString = "I am Bestinterviewquestion.com";

$searchedString = "am";



if( strpos( $mainString, $searchedString ) !== false) {

    echo "\"am\" exists in the main string";

} 
die;

$var1 = "This is good interview Question";
echo strlen($var1);

$array = array('5','2','8','4');

rsort($array);

echo $array[0];

$originalArray = array( 'ram', 'sita', 'luxman', 'hanuman', 'ravan' );
$newArray = array( 'kansh' );
//array_splice( $originalArray, 3, 0, $newArray);// add
array_splice($originalArray, 1, 2); // remove 
print_r($originalArray);die;

$dynamic = [
    'number' => 7,
    'live' => 'House',
    'drive' => 'Car',
    [
        'mow' => 'grass',
        [
            'tractor' => 'John Deere',
            'tractor2' => 'Kubota',
            'tractor3' => 'New Holland'
        ],
        'landscape' => 'mulch'
    ]
];
 
$one = is_array($dynamic);
 
$two = is_array($dynamic['number']);
 
$three = is_array($dynamic[0]);
 
echo $one ? 'The $dynamic variable is an array<br>' : 'The $dynamic variable is not an array<br>';
echo $two ? 'The "number" key of the $dynamic variable is an array<br>' : 'The "number" key of the $dynamic variable is not an array<br>';
echo $three ? 'The 0 index of the $dynamic variable is an array<br>' : 'The 0 index of the $dynamic variable is not an array<br>';
 
 
 die;

$a = array("abid","Raza","Abbas");
$b = array("ab","cd","ef");
print_r(array_combine($a, $b));



$a = "PHP";
$a = $a + 1;
echo $a;die;
$a= array('0'=>'z2','1'=>'z1','2'=>'z4','3'=>'z5','4'=>'z3');

sort($a);
print_r($a);
die;
$array=array('2','4','8','5','1','7','0', '6','9','10','3');

echo "Unsorted array is: ";
echo "<br />";
print_r($array);
echo "<br />";echo "<br />";


for($i = 0; $i < count($array); $i ++) {
    for($j = 0; $j < count($array)-1; $j ++){

        if($array[$j] > $array[$j+1]) {
            $temp = $array[$j+1];
            $array[$j+1]=$array[$j];
            $array[$j]=$temp;
        }       
    }
}

echo "Sorted Array is: ";
echo "<br />";
print_r($array);



/*
SELECT MAX(<numeric column>) FROM <table>;
SELECT MAX(<numeric column>) FROM <table> GROUP BY <other column>;
*/

?>     
