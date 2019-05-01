# Refresh From Database

This package adds a method and a button to the tearoff window which refreshes from the database. The default refresh button only refreshes from the dom.

## History

Release | Notes
--------|--------
[v1.5](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.5) | Bug fixes
[v1.4](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.4) | Bug fixes
[v1.3](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.3) | Verified for 11.0 SP15
[v1.2](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.2) | Update to 11.0 SP12
[v1.1](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.1) | Update to 11.0 SP11
[v1.0](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.0) | Initial Release

#### Supported Aras Versions
Project | Aras
--------|--------
[v1.5](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.5) | 11.0 SP15, 11.0 SP12
[v1.4](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.4) | 11.0 SP15, 11.0 SP12
[v1.3](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.3) | 11.0 SP15, 11.0 SP12
[v1.2](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.2) | 11.0 SP12
[v1.1](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.1) | 11.0 SP11
[v1.0](https://github.com/ArasLabs/refresh-from-database/releases/tag/v1.0) | 11.0 SP10

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 11.0 SPx preferred)
2. Aras Package Import tool
3. RunClientMethod import package

### Install Steps

#### Code tree Installation
These code tree changes only contain a custom icon for the toolbar. If you wish to use your own icon, you may replace the .svg file in the `\Innovator\` folder with your own.

1. Backup your code tree and store the archive in a safe place
2. Navigate to your local `..\RefreshFromDatabase\` folder
3. Copy the `\Innovator\` folder 
4. Paste this at the root of your install directory
+ By default this is `C:\Program Files\Aras\Innovator\`

#### Database Installation
1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\RefreshFromDatabase\Import\imports.mf` file in the Manifest File field.
6. Select **aras.labs.RefreshFromDatabase** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.

You are now ready to login to Aras and try out the Refresh From Database button.

## Usage

1. Log in to Aras as admin.
2. Open any item.
3. Confirm there is an additional refresh button next to the default refresh button.
4. When you want to refresh an item to see content another user has edited, you may click this new button to refresh the item with information from the database.


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Original Aras community project written by Christopher Gillis at Aras Corp.

Documented and published by Eli Donahue for Aras Labs. @cgillis-aras

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.