//виводити thank you massage and close and clear form after 1.5seconds
on_sent_ok:  $('.formTitle+p').css('display', 'none');setTimeout(function(){ $.fancybox.close(); }, 1500);setTimeout(function(){ $('.formTitle+p').css('display', 'block'); }, 2000);setTimeout(function(){ $('.wpcf7-mail-sent-ok').css('display', 'none'); }, 2000);


//виводити thankyou massage і закривати форму після вдалого відправлення повідомлення
on_sent_ok:  $('.formTitle+p').css('display', 'none');setTimeout(function(){ $.fancybox.close(); }, 1500);

//Закривати popup після відправки форми (вставляємо в форму additional setting)
on_sent_ok: $.fancybox.close();

//Зразок вставки форми
<a class="fancybox-inline btnPopUp" href="#contact_form_pop">こちら</a>

<div id="fancybox-overlay" class="fancybox-hidden" style="display: none;">
  <div id="contact_form_pop">[contact-form-7 id="76" title="Send email"]</div>
</div>

//видалити атрибут, який блокує перевірки на required
$('.wpcf7-form').removeAttr('novalidate');

//додаємо атрибути required
$('.input, input[name=radio-74]').prop( "required", true);
