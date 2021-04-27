# UTD-CS4367-MP2
MP2 Repos for CS 4367

## Part 1:
The source code is stored in `AndroidInstrument.java`
Executing the class will produce output:
```Soot started on Tue Apr 27 00:43:35 CDT 2021
dxv180004
dxv180004
dxv180004
[main] INFO soot.toDex.DexPrinter - Writing APK to "sootOutput\sq3.apk".
[main] INFO soot.toDex.DexPrinter - Do not forget to sign the .apk file with jarsigner and to align it with zipalign
Soot finished on Tue Apr 27 00:43:38 CDT 2021
Soot has run for 0 min. 3 sec.
```
## Part 2:
### Generate Keystore
The keystore is saved in `my.keystore`. The keystore's password is `12345678`, the keystore's alias is `app`

### Zipalign
The `sq3.apk` is zipligned into `my-aligned.apk`

### Sign & Verify
`sq3.apk` can now be signed and verified by `jarsigner`. This step produces an output:
```$ jarsigner -verify -verbose sq3.apk

s       5135 Mon Apr 26 23:16:38 CDT 2021 META-INF/MANIFEST.MF
        5254 Mon Apr 26 23:16:40 CDT 2021 META-INF/APP.SF
        1311 Mon Apr 26 23:16:40 CDT 2021 META-INF/APP.RSA
sm       483 Mon Apr 26 22:35:20 CDT 2021 res/drawable/action_about.png
sm       723 Mon Apr 26 22:35:20 CDT 2021 res/drawable/action_search.png
sm       429 Mon Apr 26 22:35:20 CDT 2021 res/drawable/action_settings.png
sm       684 Mon Apr 26 22:35:20 CDT 2021 res/drawable/content_discard.png
sm       841 Mon Apr 26 22:35:20 CDT 2021 res/drawable/content_edit.png
sm       399 Mon Apr 26 22:35:20 CDT 2021 res/drawable/content_email.png
sm       203 Mon Apr 26 22:35:20 CDT 2021 res/drawable/content_new.png
sm       246 Mon Apr 26 22:35:20 CDT 2021 res/drawable/content_remove.png
sm      1686 Mon Apr 26 22:35:20 CDT 2021 res/drawable/database.png
sm      2281 Mon Apr 26 22:35:20 CDT 2021 res/drawable/folder.png
sm      1912 Mon Apr 26 22:35:20 CDT 2021 res/layout/about.xml
sm      2612 Mon Apr 26 22:35:20 CDT 2021 res/layout/apps.xml
sm      1356 Mon Apr 26 22:35:20 CDT 2021 res/layout/bookmarks.xml
sm      2332 Mon Apr 26 22:35:20 CDT 2021 res/layout/browser.xml
sm      3512 Mon Apr 26 22:35:20 CDT 2021 res/layout/database_list.xml
sm      1272 Mon Apr 26 22:35:20 CDT 2021 res/layout/database_records.xml
sm      1144 Mon Apr 26 22:35:20 CDT 2021 res/layout/database_tables.xml
sm      2236 Mon Apr 26 22:35:20 CDT 2021 res/layout/filter.xml
sm      1240 Mon Apr 26 22:35:20 CDT 2021 res/layout/fragment_tabs_pager.xml
sm      1476 Mon Apr 26 22:35:20 CDT 2021 res/layout/list_item_app.xml
sm      1480 Mon Apr 26 22:35:20 CDT 2021 res/layout/list_item_bookmark.xml
sm      1984 Mon Apr 26 22:35:20 CDT 2021 res/layout/list_item_details.xml
sm      1172 Mon Apr 26 22:35:20 CDT 2021 res/layout/list_item_simple.xml
sm      1380 Mon Apr 26 22:35:20 CDT 2021 res/layout/recent.xml
sm       892 Mon Apr 26 22:35:20 CDT 2021 res/layout/tab_view.xml
sm       936 Mon Apr 26 22:35:20 CDT 2021 res/layout/table_list_item.xml
sm      1604 Mon Apr 26 22:35:20 CDT 2021 res/layout/table_record.xml
sm      1464 Mon Apr 26 22:35:20 CDT 2021 res/xml/preferences.xml
sm      3484 Mon Apr 26 22:35:20 CDT 2021 AndroidManifest.xml
sm     13296 Mon Apr 26 22:35:20 CDT 2021 resources.arsc
sm      2388 Mon Apr 26 22:35:20 CDT 2021 res/layout-v11/about.xml
sm      2404 Mon Apr 26 22:35:20 CDT 2021 res/layout-v11/filter.xml
sm      1772 Mon Apr 26 22:35:20 CDT 2021 res/layout-v11/table_record.xml
sm       687 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/action_about.png
sm      1074 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/action_search.png
sm       510 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/action_settings.png
sm       949 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/content_discard.png
sm      1166 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/content_edit.png
sm       450 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/content_email.png
sm       223 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/content_new.png
sm       331 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/content_remove.png
sm      3488 Mon Apr 26 22:35:20 CDT 2021 res/drawable-hdpi/database.png
sm      1044 Mon Apr 26 22:35:20 CDT 2021 res/drawable-ldpi/database.png
sm       483 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/action_about.png
sm       723 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/action_search.png
sm       429 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/action_settings.png
sm       684 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/content_discard.png
sm       841 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/content_edit.png
sm       399 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/content_email.png
sm       203 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/content_new.png
sm       246 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/content_remove.png
sm      1686 Mon Apr 26 22:35:20 CDT 2021 res/drawable-mdpi/database.png
sm       978 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/action_about.png
sm      1327 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/action_search.png
sm       556 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/action_settings.png
sm      1158 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/content_discard.png
sm      1545 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/content_edit.png
sm       529 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/content_email.png
sm       251 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/content_new.png
sm       352 Mon Apr 26 22:35:20 CDT 2021 res/drawable-xhdpi/content_remove.png
sm    322920 Mon Apr 26 22:35:20 CDT 2021 classes.dex

  s = signature was verified
  m = entry is listed in manifest
  k = at least one certificate was found in keystore
  i = at least one certificate was found in identity scope

- Signed by "CN=Danh, OU=CS4367, O=CS, L=Dallas, ST=Texas, C=US"
    Digest algorithm: SHA1 (weak)
    Signature algorithm: SHA1withRSA (weak), 2048-bit key

jar verified.

Warning:
This jar contains entries whose certificate chain is invalid. Reason: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
This jar contains entries whose signer certificate is self-signed.
The SHA1 digest algorithm is considered a security risk. This algorithm will be disabled in a future update.
The SHA1withRSA signature algorithm is considered a security risk. This algorithm will be disabled in a future update.
This jar contains signatures that do not include a timestamp. Without a timestamp, users may not be able to validate this jar after any of the signer certificates expire (as early as 2048-09-11).

Re-run with the -verbose and -certs options for more details.

The signer certificate will expire on 2048-09-11.
```
