# Usage Flipper — Privacy Policy

**Effective date:** 15 October 2026

Usage Flipper is a browser extension that displays usage allowances and reset times for supported AI services in small, optional floating widgets.

## Information the extension accesses

When you enable a supported integration, Usage Flipper communicates with that AI provider to request information such as remaining usage percentages, allowance windows, and reset times. Where supported, it uses the provider session already signed in through your browser. The provider may process these requests under its own privacy policy.

To request usage information, the extension may need to access authentication or session information available in the browser. **You should not need to enter your AI account password into Usage Flipper.** Session and authentication details are not intended to be sent to a Usage Flipper-operated server.

Only providers with working integrations can supply live usage information. Displaying a provider during setup does not mean its integration is already available.

## Information stored on your device

Usage Flipper uses browser extension storage to save settings such as your selected services, which floating widgets are enabled, their positions, layout choices, and other display preferences. It may also cache retrieved allowance figures, reset timestamps, and connection status so the interface remains useful between refreshes.

The extension is designed to keep these settings and cached readings in the browser rather than upload them to a Usage Flipper account or proprietary server.

## Websites and permissions

When enabled, Usage Flipper inserts an interactive floating usage widget into supported webpages. This requires access to webpages where the widget is displayed.

Provider-domain permissions allow the extension to request usage data from the relevant service. Usage Flipper does not need to collect the contents of your chats, documents, or unrelated webpages to perform its stated purpose.

## Sharing, selling and tracking

Usage Flipper does not operate a separate user account or advertising service. It is not designed to sell usage information, share it with data brokers, or use it for targeted advertising.

Requests to AI providers are necessary to retrieve allowance details and are subject to those providers' own practices. The extension also relies on the browser's normal extension infrastructure.

## Your choices and deleting local data

You can turn floating widgets on or off and change your chosen providers through the extension controls.

To remove locally saved settings and cached usage details, uninstall Usage Flipper from your browser. Depending on the browser and sync settings, you may also need to clear synchronised extension data.

You can sign out of a connected AI provider to stop that browser session being used for its usage requests.

## Security and limitations

Usage Flipper is an independent tool, not an official product of OpenAI, Anthropic, Cursor, xAI, Google, or other AI providers. Integrations using provider interfaces can change or become unavailable without notice.

## Changes to this policy

We may update this policy as features, integrations, permissions or data practices change. The updated date and text will be published in this repository.

## Contact

For privacy questions, support or concerns, please open an issue at:

https://github.com/smo82-dev/UsageFlipper/issues

**Note for release:** This policy describes the intended behaviour of the extension. Before publication, its statements should be checked against the exact extension ZIP being submitted, especially session handling, storage, requested website permissions and any additional integrations.
