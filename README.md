# Additional files for building /e/

Add this repo to the manifest and place it in "vendor/extra/".

The only purpose for this repo right now is to change the OTA URL. In case this works already with the build arg,
this repo does not have to be used.

## Custom OTA URL set in "product.mk"

See this info from reddit: https://www.reddit.com/r/LineageOS/comments/c38itu/configuring_the_lineage_ota_updater/

> you can either do that with a property PRODUCT_PROPERTY_OVERRIDES += lineage.updater.uri=https://updater.example.com/api/v1/{device}/{type}/{incr} 
> or with an overlay <string name="update_server_url" translatable="false">https://updater.example.com/api/v1/{device}/{type}/{incr}</string>
> 
> here are examples for both 
> 
> https://github.com/Stricted/android_vendor_extra/blob/lineage-15.1/product.mk#L16 
> 
> https://github.com/Stricted/android_vendor_extra/blob/lineage-15.1/overlay/packages/apps/Updater/strings.xml#L2

# License

Check file "LICENSE".
