# Popup
For Popup Display Script 


<script>
    require(
        [
            'jquery',
            'Magento_Ui/js/modal/modal'
        ],
        function($, modal) {
            var options = {
                buttons: [{
                    text: $.mage.__('Close'),
                    class: 'modal-close',
                    click: function (){
                        this.closeModal();
                    }
                }]
            };

            modal(options, $('#popup-newsletter'));
                $("#popup-newsletter").modal("openModal");
        }
    );
</script>
