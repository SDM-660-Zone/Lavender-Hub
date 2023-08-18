# Know Issues
* Issues recognized by me and workarounds for now;

## Redmi Note 7 - Lavender

|Issue|Description|Workaround|
|-----|-----|-----|
|Play L1 Content|After updated our DRM stack for 4.19 our liboemcrypto blobs aren't able to play DRM protected content anymore even displaying L1 support a black screen would be presented instead of content|We are using L3 for now which is working just fine|
|Recovery Decryption|We aren't able to decrypt userdata on 4.19 on custom recovery's for now|None (Decrypt data by default isn't an option)|
|Quick Torch Usage|When this feature it's enabled power button may can fail to wakeup, at single touch.|Disable the feature and it will work as always did.|
