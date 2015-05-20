## Yii QRCode
Original PHP QRCode is from [http://phpqrcode.sourceforge.net/](http://phpqrcode.sourceforge.net/) writed by deltalab@poczta.fm

I convert it to make it easier to use in Yii framework.
Hope useful to you.

## Requirements
* Yii 1.x 
* PHP 5.x

## Installation
* Place this extension in /protected/extensions/qrcode
* In main.php, add the following to 'components':

```php
'qrcode' => array(
    'class' => 'ext.qrcode.QRCode',
),
```

## Usage
examples

```php
#create text qrcode
Yii::app()->qrcode->create('test');
#create link qrcode
Yii::app()->qrcode->create('http://www.wanzhoumo.com');
#set qrcode size
Yii::app()->qrcode->setSize(6)->create('test');
```

## License
Modified BSD License <https://github.com/jianzhenchen/Yii-QRcode>