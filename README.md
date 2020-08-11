# Codeigniter-Barcode


> Codeigniter-Barcode by Zend Library - Changelog & Documentation


[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/desta88/Codeigniter-Barcode/graphs/commit-activity)
[![Github all releases](https://img.shields.io/github/downloads/desta88/Codeigniter-Barcode/total.svg)](https://GitHub.com/desta88/Codeigniter-Barcode/releases/)
[![HitCount](http://hits.dwyl.com/desta88/https://githubcom/desta88/Codeigniter-Barcode.svg)](http://hits.dwyl.com/desta88/https://githubcom/desta88/Codeigniter-Barcode)


[![GitHub forks](https://img.shields.io/github/forks/desta88/Codeigniter-Barcode.svg?style=social&label=Fork&maxAge=2592000)](https://GitHub.com/desta88/Codeigniter-Barcode/network/)
[![GitHub stars](https://img.shields.io/github/stars/desta88/Codeigniter-Barcode.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/desta88/Codeigniter-Barcode/stargazers/)


Create barcode generator using Zend Library

It's so easy to use, you just extract the library into libraries path and then put library in controller, check it out now!




Installation
------------
1. Download and extract into libraries path<br>
2. Include your library in controller




Usage
------------
```
class Main extends CI_Controller {

	public function index()
	{
		// You can put anything here to generate of barcode
		$string = 'code39';
		$this->set_barcode($string);
	}
	
	private function set_barcode($code)
	{
		// Load library
		$this->load->library('zend');
		// Load in folder Zend
		$this->zend->load('Zend/Barcode');
		// Generate barcode
		Zend_Barcode::render('code128', 'image', array('text'=>$code), array());
	}
	
}
```


Changelog Update 
----------------
#v1.0 Release




License
------------
License : [MIT License](https://github.com/desta88/Codeigniter-Barcode/blob/master/LICENSE)


Authors
------------
Official Authors [@desta](https://mdcreative.id/)
