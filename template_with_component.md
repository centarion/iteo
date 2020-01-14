## Пример шаблона с вставленным стандартным компонентом
```
<?
require($_SERVER["DOCUMENT_ROOT"]."/bitrix/header.php");
$APPLICATION->SetPageProperty("description", "Новости");
$APPLICATION->SetPageProperty("title", "Новости");
$APPLICATION->SetTitle("Новости");
?>

<!-- Код HTML до компонента -->

<?$APPLICATION->IncludeComponent(
    "bitrix:news.list", 
    "news", 
    array(
         // Параметры компонента
    ),
    false
);
?>

<!-- Код HTML после компонента -->

<?require($_SERVER["DOCUMENT_ROOT"]."/bitrix/footer.php");?>
```
