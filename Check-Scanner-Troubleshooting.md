# Check Scanner Troubleshooting

## Audience

Helpdesk technicians

## Purpose
 
This procedure applies when the banking website does not detect the installed check scanner. It applies to most Digital Check CheXpress and TellerScan Check Scanner models.

## Expected Result

The banking website loads without scanner related error message. When the user clicks Scan within the banking website, the check is successfully scanned and uploaded.


## Notes:

Running the test from Ranger Flex may restore functionality even if the test scan fails.

## Steps:

### Initial troubleshooting:

1. Open the Ranger Flex Program.
2. Verify the "Silver Bullet" splash screen appears.
3. Run the test in the program.
4. Close the program regardless of results.
5. Have the user test.

### Advanced Remediation

6. Disconnect the scanner from USB and power cables.
7. Uninstall device.
8. Check the Device Manager for hidden or ghost devices and remove any related entries.
9. Check the Registry for any persistent keys and remove any entries
10. Uninstall all related software.
11. Reinstall drivers and software.
12. Do not reconnect the scanner USB and power cables until the installer instructs you. 
13. Have the user test.

### Pre-Escalation Verification

14. Recheck Device Manager for ghost devices and remove any found.
15. Recheck the Registry for persistent entries and remove any found.
16. Uninstall and reinstall all scanner drivers and software again.
17. Have the user test the scanner.

## Escalation

If the issue remains unresolved after completing all troubleshooting steps, contact the scanner manufacturer for further remediation. 
