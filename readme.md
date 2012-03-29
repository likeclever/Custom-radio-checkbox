﻿Custom radio & checkbox jQuery plugin;
by N0r8 millianorb@gmail.com;

	usage:
	$('your checkbox or radio selector').Custom({
		customStyleClass:'classForcustomView',
		customHeight:'height of checkbox or radio'
	});
	
	example:
	$('input[type="checkbox"]').Custom({
		customStyleClass:'checkbox',
		customHeight:'16'
	});
	
	If you need disable or enable button update them like this(in demo.html):
	
	$('#radio3').removeAttr('disabled').trigger('custom.refresh');
	
	If you dinamical added button just recall plugin after html with buttons added(in demo.html):
	
		$('#create').html('<input type="radio" id="radio4" name="group" class="radioclass"/><label for="radio4">radio4</label><input type="checkbox" id="checkbox4" class="checkboxclass"/><label for="checkbox4">checkbox4</label><br clear="all" style="clear:both;"/>')
		$(".radioclass").Custom({
			customStyleClass:'radio',
			customHeight:'25'
		});
		$(".checkboxclass").Custom({
			customStyleClass:'checkbox',
			customHeight:'20'
		});