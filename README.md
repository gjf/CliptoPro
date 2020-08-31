This is very simple and stupid module to give CliptoPro application (https://play.google.com/store/apps/details?id=com.wb.clipboard.pro) all necessary permission to access clipboard on latest Android.

Sure the user can do it using adb commands, but this module do it automatically without PC.

You can install the module and no reboot. There will be a new module in Magisk after that, but it will disappear on next reboot - this is normal, because all correct permissions are granted and stored during install.

## Requirements ##
- CliptoPro application. Otherwise it is useless.

## Details ##
In fact the following commands are executed:
pm grant com.wb.clipboard.pro android.permission.READ_LOGS
appops set com.wb.clipboard.pro SYSTEM_ALERT_WINDOW allow
am force-stop com.wb.clipboard.pro

## ChangeLog ##
* v.1 First Release (and possibly the last)