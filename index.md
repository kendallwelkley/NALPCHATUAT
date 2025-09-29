<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
window.addEventListener("onEmbeddedMessagingReady", e => {
						  embeddedservice_bootstrap.prechatAPI.setVisiblePrechatFields({
						    // List the pre-chat field names with the value and whether
						    // it's editable in the pre-chat form.
		 						"_email": {
						      	"value": "TEST12@gmail.com",
						      	"isEditableByEndUser": false
						    	},
							 	"Account_Code": {
						      	"value": "11111",
						      	"isEditableByEndUser": false
								},
								"_firstName": {
						      	"value": "First",
						      	"isEditableByEndUser": true
						    	},
		 						"_lastName": {
						      	"value": "Last",
						      	"isEditableByEndUser": true
						    	},
		 				  });
                          
						});
			embeddedservice_bootstrap.init(
				'00DU70000086JPx',
				'Customer_Support_1',
				'https://fleetcorna--uat.sandbox.my.site.com/ESWCustomerSupport1758745136326',
				{
					scrt2URL: 'https://fleetcorna--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://fleetcorna--uat.sandbox.my.site.com/ESWCustomerSupport1758745136326/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
