# Простейший шаблон для страницы в Битрикс
```
<?
require($_SERVER["DOCUMENT_ROOT"]."/bitrix/header.php");
$APPLICATION->SetPageProperty("description", "О компании");
$APPLICATION->SetPageProperty("title", "О компании");
$APPLICATION->SetTitle("О компании");
?>

<!-- Здесь нужно писать код на HTML. -->

<!-- Вставка заголовка страницы -->
<?=$APPLICATION->GetTitle() ?>

<!-- Здесь нужно писать код на HTML. -->

<?require($_SERVER["DOCUMENT_ROOT"]."/bitrix/footer.php");?>
```
