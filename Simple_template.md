# Простейший шаблон для страницы в Битрикс
<code>
<?
require($_SERVER["DOCUMENT_ROOT"]."/bitrix/header.php");
$APPLICATION->SetPageProperty("description", "О компании");
$APPLICATION->SetPageProperty("title", "О компании");
$APPLICATION->SetTitle("О компании");
?>

<?=$APPLICATION->GetTitle() ?>

<!-- Здесь нужно писать код на HTML. -->

<?require($_SERVER["DOCUMENT_ROOT"]."/bitrix/footer.php");?>
</code>
