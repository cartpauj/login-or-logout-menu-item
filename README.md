# Login or Logout Menu Item

Add a dynamic "Login" or "Logout" menu item to any WordPress menu. The link automatically switches based on whether the visitor is logged in or out.

Works with both **classic menus** (Appearance > Menus) and the **block editor Navigation block**.

## Features

- Dynamic menu item that shows "Login" or "Logout" depending on user state
- Configurable login page URL, login redirect URL, and logout redirect URL
- Classic menu support via the Login/Logout meta box
- Block editor Navigation block support — search "login" or "logout" in the link picker
- Admin settings page at **Settings > Login or Logout**
- Administrators are excluded from login redirects

## Installation

Install from the [WordPress Plugin Directory](https://wordpress.org/plugins/login-or-logout-menu-item/), or:

1. Download the latest release zip from the [Releases page](https://github.com/cartpauj/login-or-logout-menu-item/releases)
2. In your WordPress dashboard go to **Plugins > Add New > Upload Plugin**
3. Upload the zip and activate

## Usage

### Classic Menus

1. Go to **Appearance > Menus**
2. Open **Screen Options** (top right) and check **Login/Logout**
3. In the left sidebar, expand **Login/Logout** and add **Login|Logout** to your menu
4. Save the menu

The URL must remain `#lolmiloginout#`. You can customize the label — just keep the `|` separating the logged-out and logged-in text (e.g. `Sign In|Sign Out`).

### Navigation Block

1. Add or edit a Navigation block in the page/site editor
2. Click (+) to add a new link
3. Search for "login" or "logout"
4. Select **Login|Logout** from the suggestions

### Settings

Configure redirect URLs at **Settings > Login or Logout**:

- **Login Page URL** — Where your login page lives (default: `/wp-login.php`)
- **Login Redirect URL** — Where to send users after login (default: home page)
- **Logout Redirect URL** — Where to send users after logout (default: home page)

## Troubleshooting

**Menu still shows "Login" after logging in (or vice versa)** — Usually a caching issue. Disable page caching for logged-in users and turn off browser caching in your caching plugin (Cloudflare, WP Rocket, etc.).

**Login redirects somewhere unexpected** — Another plugin (e.g. MemberPress) may be overriding the redirect. Configure the redirect in that plugin instead.

## Credits

Based on the BAW Login/Logout Menu plugin by Juliobox.

## License

GPLv3 — see [LICENSE](LICENSE) for details.
