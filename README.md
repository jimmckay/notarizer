# notarizer

#### Notarize and Staple App or DMG

**Usage:**
  **notarizer -u username -p password [options] FILE**
  **notarizer --get-providers -u username**

FILE will be uploaded to Apple's notary service and stapled on success.

Options:
- **-u, --username** [username] (required)
   The username associated with your developer account
- **-p, --password** [password] (required)
   The password for the username. Can use @keychain:ITEM to access password stored in login keychain with service name ITEM.
   See [App-Specific Passwords](https://support.apple.com/en-us/HT204397) for help.
- **-i, --itc-provider** [itc_provider_id]
   The developer shortname to use (usually your App Store Connect id without spaces or '|'s)
- **-s, --sign** [cerificatename]
   An optional cerificate for codesigning before notarization
- **-n, --notify**
   If present, a dialog will be displayed on completion
- **--get-providers**
   Request a listing of provider shortnames
- **-h, --help**
   Show this message and exit
- **-v, --version**
   Print version information and exit

   Written by Jim McKay 
   Copyright 2019
   
   With some ideas from [Thom McGrath's Code](https://github.com/thommcgrath/Beacon/blob/master/Installers/Mac/Build.sh "Thom McGrath's Code")

