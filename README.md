It implements CKEditor and KCFinder with easy to use parameters.

Download it to your extensions folder and you can use it as follows :

	$this->widget('application.extensions.editor.CKkceditor',array(
        "model"=>$model,                # Data-Model
        "attribute"=>'descripcion',         # Attribute in the Data-Model
        "height"=>'400px',
        "width"=>'100%',
            "filespath"=>(!$model->isNewRecord)?Yii::app()->basePath."/../media/paquetes/".$model->idpaquete."/":"",
            "filesurl"=>(!$model->isNewRecord)?Yii::app()->baseUrl."/media/paquetes/".$model->idpaquete."/":"",
    ) );

If you want to contribute please just ask; I do this on my free time so all the help is appreciated.