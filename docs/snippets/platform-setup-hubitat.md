=== "Hubitat"
    1. Navigate to the product's GitHub repository (see above).
    1. Navigate to ==Releases==.
    1. Right click on the hubitat-bundle.zip and copy the link.
    1. In Hubitat, navigate to ==Bundles== in the left-side menu (expand the **For Developers** section if you do not see **Bundles**, or turn on **Enabled advanced/developer options** in **Settings** if you do not see the **For Developers** section).
    1. Select the ==Import ZIP== button (towards the top of the page).
    1. Select ==Import from URL== and paste the copied link into ==URL to import bundle from==. Leave all other settings as default.
    1. Select ==Import== and wait for the process to finish. The text **Bundle imported** will appear at the bottom of the dialog when the process is complete, and the dialog with close shortly afterwards. You will then see the bundle in the table on the **Bundles** page.
    1. Next, navigate to ==Devices==.
    1. Select ==Add device==.
    1. Under ==Add device manually==, select ==Virtual==.
    1. Using the drop-down, search for ==Elevated Sensors== and select your device (e.g. ==Elevated Sensors Bed Presence Mk1==).
    1. Select ==Next==.
    1. Name your device and select ==Next==.
    1. Select a room and select ==Next==.
    1. Select ==View device details==.
    1. Under ==Preferences==, enter the ==Device IP Address== (this can be an IP address or mDNS address) and hit ==Save Preferences==.
    1. Your device is ready to use!
