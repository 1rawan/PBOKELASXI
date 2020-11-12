<?php
class mobil
{
    private $warna;
    public $tipe;
    public $jenis;
    public $ukuran;


    public function __construct($warna, $tipe, $jenis, $ukuran)
    {
        $this->warna = $warna;
        $this->tipe = $tipe;
        $this->jenis = $jenis;
        $this->ukuran = $ukuran;
        
    }
    public function tampil1()
    {
        return "$this->warna,$this->tipe,$this->jenis,$this->ukuran";
    }
    public function tampil2()
    {
        return "$this->warna,$this->tipe,$this->jenis,$this->ukuran";
    }
    public function getwarna()
    {
        return $this->warna;
    }
    public function setwarna($warna){
        $this->warna = $warna;
    }
}
//================================================================ inheritens private,public

class turbo extends mobil
{
    private $model;

    public function __construct($warna, $tipe, $jenis, $ukuran, $model)
    {

        $this->warna = $warna;
        $this->tipe = $tipe;
        $this->jenis = $jenis;
        $this->ukuran = $ukuran;
        $this->model = $model;
    }

    public function cetaksemua()
    {
        $str = "Mobilbalap : {$this->tampil2()} {$this->model}";
        //$str = "Mobilbalap : " . parent::cetaksemua() . " {$this->model}";
        return $str;
    }
}
//================================================================= protected
class klasik extends mobil
{
    protected $kondisi;

    public function __construct($warna, $tipe, $jenis, $ukuran, $kondisi)
    {

        $this->warna = $warna;
        $this->tipe = $tipe;
        $this->jenis = $jenis;
        $this->ukuran = $ukuran;
        $this->kondisi = $kondisi;
    }

    public function cetaksemua()
    {
        $str = "Mobil kuno : {$this->tampil2()} {$this->kondisi}";
        //$str = "Mobil kuno : " . parent::cetaksemua() . " {$this->kondisi}";
        return $str;
    }
}
//======================================================================
$mobil_toyota1 = new klasik("hijau", "mini coper", "mini", "kecil", "karatan");
echo $mobil_toyota1->cetaksemua();
echo "</br>";

$mobil_toyota1 = new turbo("merah", "mini bus", "bus", "besar", "sport");
echo $mobil_toyota1->cetaksemua();

echo "</br>";
$mobilasli = new mobil("hitam", "minibus", "sedan", "kecil", 1);
echo $mobilasli->tampil1();


echo "</br>";
echo $mobilasli->setwarna("ungu - unguan");
echo $mobilasli->getwarna();


// echo "</br>";
// $mobil_toyota2 = new mobil();
// echo $mobil_toyota2->bodol;
