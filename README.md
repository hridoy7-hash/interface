# interface

<?php
interface School{
    public function mySchool();
}
interface Collage{
    public function mySchool();
}
interface Varsity{
    public function mySchool();
}
class Teacher implements School,Collage,Varsity{
    public function __construct(){
        $this->mySchool();
        $this->myCollage();
        $this->myVarsity();


    }
    public function mySchool(){
        echo "I am a School Teacher";
        echo "<br/>";
    }
    
    public function myCollage(){
        echo "I am a Collage Teacher";
        echo "<br/>";
    }
    
    public function myVarsity(){
        echo "I am a Varsity Teacher";
        echo "<br/>";
    }
}


class Student implements School,Collage,Varsity{
    public function __construct(){
        $this->mySchool();
        $this->myCollage();
        $this->myVarsity();


    }
    public function mySchool(){
        echo "I am a School Student";
        echo "<br/>";
    }
    
    public function myCollage(){
        echo "I am a Collage Student";
        echo "<br/>";
    }
    
    public function myVarsity(){
        echo "I am a Varsity Student";
    }
}


$teacher= new Teacher();
$student=new Student();





?>
