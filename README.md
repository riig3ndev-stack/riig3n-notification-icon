# riig3n_notification_icon

Android resources for RiiG3N: the push notification icon and the Chameleon Mode
disguise launcher icons. Nothing else.

- `@drawable/ic_stat_riig3n` - the white chameleon silhouette used as the small
  notification icon (mdpi to xxxhdpi, 24dp with 2dp padding).
- `@color/riig3n_notification_accent` - the accent colour (#E30045).

The app points Firebase Messaging at them with two `<meta-data>` entries in its
AndroidManifest (`com.google.firebase.messaging.default_notification_icon` and
`com.google.firebase.messaging.default_notification_color`).

Disguise launcher icons (Chameleon Mode), used by activity-aliases in the app:

- `@mipmap/ic_disguise_driver`, `ic_disguise_gloss`, `ic_disguise_trader`,
  `ic_disguise_myjog` - adaptive icons, plus `_round` and legacy PNGs at every
  density. Original designs, not based on any real app.
- `@string/disguise_driver_label`, `disguise_gloss_label`,
  `disguise_trader_label`, `disguise_myjog_label` - the names shown under each
  icon (Driver, Gloss, Trader, My Jog).

The Android plugin class does nothing; it only exists so Flutter includes this
library (and its resources) in the Android build. iOS and web are untouched.
