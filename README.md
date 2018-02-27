
# UnityMobilePermissionManager
iOS & Android permissions check / request

For Android use this library https://github.com/sanukin39/UniAndroidPermission

Currently WIP.

## Installation
Simply copy this library to YourProject/Assets

## Check for permission
Check permission returns an int, 1 when allowed, 0 otherwise.

Usage :

    int permission = iOSPermissions.CheckPermission (iOSPermissions.PERMISSION.CAMERA)

Supported permissions :
 - CAMERA
 - GEOLOCATION
 - ... more to come

## Request a permission
Request a permission, needing the gameobject and the callback function name as parameter. The callback function returns 1 when allowed, 0 otherwise.

    iOSPermissions.RequestPermission(gameObject.name, "PermissionCallback");
    
    private void PermissionCallback(int allowed){
	    // 1 if allowed, 0 otherwise
    }
Supported permissions :
 - CAMERA
 - ... more to come



