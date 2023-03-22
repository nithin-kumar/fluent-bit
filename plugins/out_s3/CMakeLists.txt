set(src
  s3.c
  s3_store.c
  s3_multipart.c)

FLB_PLUGIN(out_s3 "${src}" "")
target_link_libraries(flb-plugin-out_s3 curl)
#target_link_libraries(flb-plugin-out_s3  cjson)
target_link_libraries(flb-plugin-out_s3  jansson)
