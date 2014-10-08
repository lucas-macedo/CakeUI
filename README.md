CakeUI
======
<h2>Introduction</h2>
<p>Plugin to improve user interface of cakephp applications.</p>
<p>This plugin is based on <a href='http://getbootstrap.com/' target='_blank'>Bootstrap</a>.</p>
<h3>DOC</h3>
<p>Doc and examples page: <a href='http://cakeui-examples.2km.com.br'>http://cakeui-examples.2km.com.br</a></p>

<h2>Install / Instalação</h2>

Clone github:
<pre>
cd your_app_dir/Plugin
git clone https://github.com/2km/CakeUI.git
</pre>

Load on bootstrap.php
<pre> 
CakePlugin::load('CakeUI');
</pre>

Config AppController.php
<pre> 
public $helpers = array(
    'Form'=> array('className' => 'CakeUI.BootstrapForm'), 
    'Html'=> array('className' => 'CakeUI.BootstrapHtml')
);
public function beforeFilter(){
    $this->layout='CakeUI.default';
}
</pre>