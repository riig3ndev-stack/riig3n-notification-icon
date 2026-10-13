# riig3n_notification_icon

Android resources for RiiG3N push notifications. Nothing else.

- `@drawable/ic_stat_riig3n` - the white chameleon silhouette used as the small
  notification icon (mdpi to xxxhdpi, 24dp with 2dp padding).
- `@color/riig3n_notification_accent` - the accent colour (#E30045).

The app points Firebase Messaging at them with two `<meta-data>` entries in its
AndroidManifest (`com.google.firebase.messaging.default_notification_icon` and
`com.google.firebase.messaging.default_notification_color`).

The Android plugin class does nothing; it only exists so Flutter includes this
library (and its resources) in the Android build. iOS and web are untouched.
