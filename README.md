This module is forked from ECPay/ECPayAIO_Node.js

Add options injection ( see /ECPAY_Payment_node_js/example/ )

Usage:
```
const base_param = {...}
const inv_param = {...}

const options = {
  OperationMode: 'Test',
  MercProfile: {
    MerchantID: 'your merhant id',
    HaskKey: 'your hash key',
    HashIV: 'your hash IV'
  },
  IgnorePayment: ['CSV', 'BARCODE'],
  IsProjectContractor: false
},
  create = new ecpay_payment(options),
  html = create.payment_client.aio_check_out_all(base_param, inv_params)
```
