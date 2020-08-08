# Codeigniter-Barcode


> Codeigniter-Barcode by Zend Library - Changelog & Documentation


[![Inline docs](http://inch-ci.org/github/desta88/Codeigniter-Barcode.svg?branch=master)](http://inch-ci.org/github/desta88/Codeigniter-Barcode) 
[![HitCount](http://hits.dwyl.com/desta88/Codeigniter-Barcode.svg)](http://hits.dwyl.com/desta88/Codeigniter-Barcode)
[![Coverage Status](https://coveralls.io/repos/github/desta88/Codeigniter-Barcode/badge.svg?branch=master)](https://coveralls.io/github/desta88/Codeigniter-Barcode?branch=master)


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
		$temp = 'jh0n';
		$this->set_barcode($temp);
	}
	
	private function set_barcode($code)
	{
		//load library
		$this->load->library('zend');
		//load in folder Zend
		$this->zend->load('Zend/Barcode');
		//generate barcode
		Zend_Barcode::render('code128', 'image', array('text'=>$code), array());
	}
	
}
```


Changelog Update 
----------------
#SOON




License
------------
License : [MIT License](http://opensource.org/licenses/mit-license.html)

Authors
------------
Official Authors [@desta](https://mdcreative.id/)
