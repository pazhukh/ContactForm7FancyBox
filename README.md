//Закривати popup після відправки форми (вставляємо в форму additional setting)
on_sent_ok: $.fancybox.close();

//Зразок вставки форми
<a class="fancybox-inline btnPopUp" href="#contact_form_pop">こちら</a>

<div id="fancybox-overlay" class="fancybox-hidden" style="display: none;">
  <div id="contact_form_pop">[contact-form-7 id="76" title="Send email"]</div>
</div>
