# _Change log Adapter OCSGW_

## _`2021-06-11`_
* Sửa api: /ocs-gw/update-home-zone
    * Request cũ: 
    * ```json
            {
              "accountId": "string",
              "homeZone": "string"
            }
      ```
    * Request mới
    * ```json
      {
         "accountId": "84901778899",
         "homeZone1": "hz1",
         "homeZone2": "hz2",
         "homeZone3": "hz3",
         "homeZone4": "hz4",
         "psHomeZone1": "ps1",
         "psHomeZone2": "ps2"
      }
        ```

* Sửa api: /ocs-gw/subscribe-m-bundle
    * Request cũ: 
        * ```json
            {
              "accountId": "string",
              "accountType": "string",
              "bundleId": "string",
              "bundleList": {
                "bundleInfo": [
                  {
                    "amount": "string",
                    "bucketId": "string",
                    "index": "string",
                    "method": "string",
                    "startTime": "string",
                    "validityTime": "string"
                  }
                ]
              }
            }
          ```
    * Request mới
    * ```json
          {
            "accountId": "string",
            "accountType": "string",
            "bundleId": "string",
            "bundleList": {
              "bundleInfo": [
                {
                  "amount": "string",
                  "bucketId": "string",
                  "method": "string",
                  "startTime": "string",
                  "validityTime": "string"
                }
              ]
            }
          }
      ```
## _`2021-06-10`_
* Sửa api: /ocs-gw/adjust-main-balance
    * Request cũ: 
        * ```json
            {
              "accountId": "84901778899",
              "amount": "1000",
              "creditValidityDelta": "1",
              "method": "INCR",
              "recharge":"N"
            }
          ```
    * Request mới
    * ```json
      {
         "accountId": "84901778899",
         "amount": "1000",
         "creditValidityDelta": "1",
         "method": "INCR"
      }
      ```


