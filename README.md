PowerManagement
===============
Plugin for PhoneGap Build

Based on the work of https://github.com/simplec-dev/powermanagement but with support to reboot a device. Rebooting requires root access on your device.

The PowerManagement plugin offers access to the devices power-management functionality.
It should be used for applications which keep running for a long time without any user interaction.

For details on power functionality see:

* iOS: [idleTimerDisabled](http://developer.apple.com/library/ios/documentation/UIKit/Reference/UIApplication_Class/Reference/Reference.html#//apple_ref/occ/instp/UIApplication/idleTimerDisabled)


Using the plugin
----------------

	// prevent device from sleeping
    window.plugins.powerManagement.acquire();
    
	// allow device to sleep
    window.plugins.powerManagement.release();

    // reboot device (requires rooted device)
    window.plugins.powerManagement.reboot();
    
    