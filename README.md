# A boilerplate Manifest-3 Compliant Chrome Extension for Dart/Flutter Projects

Browser extensions are helpful in a variety of use cases. Recent changes to how Google implements Manifest (requiring Manifest 3.0 compliance for all extensions by June/July 2023) will drive a need for projects that are compliant with this format.

## Getting Started

- Clone the project
- Modify pubspec.yaml to suit your needs
- flutter pub get
- View/modify /web/manifest.json to suit your needs.
- In /web/index.html, note the size of the window reflected in the height/width of the HTML tag at the top, and set accordingly.
- To build, run `flutter build web --web-renderer html --csp`.

The build output will be in /build/web. Open Chrome, click the three dots in the upper right and do More Tools > Extensions.

![image](https://user-images.githubusercontent.com/106363211/212156894-32f0f8b5-9799-4c1a-8398-aff4b72517fe.png)

Ensure that 'Developer Mode' is enabled in the upper right corner of the Extensions tab: 

![image](https://user-images.githubusercontent.com/106363211/212157471-80f2e796-2686-484d-8ed5-3530e647087e.png)

In the upper left-hand-corner of the Extensions tab, click 'Load Unpacked'. 

![image](https://user-images.githubusercontent.com/106363211/212158220-3e41e012-7078-44fe-a51b-bad3dd9d0671.png)

Browse to <your_project_folder>/build/eeb and select that folder. The extension should then be listed in the extensions list, and ready for use.

For more information about Flutter and Chrome Extension capabilities, including how to publish to the app store, you can visit e.g. https://blog.codemagic.io/how-to-build-a-chrome-extension-with-flutter-web/.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
