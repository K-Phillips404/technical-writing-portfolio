# User Cannot Open Shared Documents (User ID Mismatch)

## Audience

Help Desk Technicians.

## Purpose

Troubleshooting guide for the user ID mismatch problem in SharePoint and/or OneDrive. This issue can be identified by the following symptoms:

- The user can no longer view files shared from OneDrive or SharePoint when signed into their Microsoft 365 account.
- They cannot view the shared files even when the files are set so anyone can view. However, they can view files shared with anyone when signed out of Microsoft 365.
- The user's OneDrive URL will have a number, usually a 1, appended to the end after the Top-Level Domain. 

### Example: 

Standard OneDrive URL: 
`https://yourdomain.sharepoint.com/personal/username_yourdomain_com`

UserID Mismatch URL: 
`https://yourdomain.sharepoint.com/personal/username_yourdomain_com1`

## Cause: 

The most common cause is the user's original account was deleted from the Microsoft 365 admin console, and a new account was created with the same User Principal Name (UPN).

## Resolution:

### Method 1: Reconnect the Existing OneDrive Site

Note: 
This is the preferred method because the user’s sign-in experience will not change.

1. Navigate to the Microsoft User ID Mismatch tool.
    - URL: `https://aka.ms/PillarSiteUserIDMismatch`
2. Paste the user's original OneDrive URL in the first box.
    - This is the URL without the "1" at the end
3. Paste the UPN in the second box.
4. Run the test.
5. Apply the recommended fix.

### Possible Outcomes:

1. The tool reconnects the user to the original OneDrive site.
    - Ensure the user can access their documents.
    - If they can, no further action is required.
    - If they cannot, proceed to Method 2.
2. The tool will ask if you want to disconnect the old ID.
    - If this outcome arises, do the following:
         1. Back up the user's documents
         2. Allow the tool to disconnect the old ID.
         3. Test the user's access
         4. Restore documents if necessary
         5. If the user cannot view shared documents, proceed to Method 2.
3. The tool returns an error message.
    - Usually, "The site could not be found."

### Method 2: UPN update.
 
1. Change the user's UPN in the Microsoft 365 admin console.
2. Set the old UPN as an alias.
3. Show the user how to sign in with the new UPN.
4. Confirm users can access shared documents.

## Warning:

If the user’s UPN is changed, documents will need to be reshared with the user. Microsoft does not automatically update URLs.

## Verification:

Confirm the following:

- The user can access shared documents while signed in.
- OneDrive and SharePoint links open successfully.
- OneDrive URL no longer has a number at the end of it.
