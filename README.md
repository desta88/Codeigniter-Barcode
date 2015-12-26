[Codeigniter Barcode Generator With Zend Library, Support CI 2 & 3](https://github.com/desta88/Codeigniter-Barcode-Generator-Zend-Library)
==========================================

Create barcode generator using Zend Library

It's so easy to use, you just extract the library into libraries path and then put library in controller, check it out now!

<h1>Setup</h1>

<blockquote>
	1. Download and extract <a href="http://api.mdesain.com/Codeigniter-Barcode-Generator-Zend-Library/barcode.zip">barcode.zip</a> into libraries path<br>
	2. Include your library in controller
</blockquote>

Here's an example:

```
class Main extends CI_Controller {

	public function index()
	{
		//I'm just using rand() function for data example
		$temp = rand(10000, 99999);
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

<strong>Example: <a href="http://api.mdesain.com/Codeigniter-Barcode-Generator-Zend-Library/">http://api.mdesain.com/Codeigniter-Barcode-Generator-Zend-Library</a></strong>
