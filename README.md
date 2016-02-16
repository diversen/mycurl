# mycurl

## Example

~~~.php
include_once "vendor/autoload.php";
use diversen\mycurl;

$c = new mycurl('http://coscms/account/login/index');
$post = array (
    'email' => 'test',
    'password' => 'test',
    'submit_account_login' => 'Send');

$c->setPost($post);
$c->createCurl();

echo $c->getWebPage();

~~~