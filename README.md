# Google Assistant Unofficial Desktop Client

![G Assist Banner](images/Banner.png)

Google Assistant Unofficial Desktop Client is a cross-platform desktop client for Google Assistant based on **Google Assistant SDK**.

> Note:
> ---
>
> The **"Google Assistant Unofficial Desktop Client"** is in `beta` and under development. So, if you find any bugs or have any suggestion, feel free to post an _issue_ or a _pull request_.

## Inspiration

The design is inspired by Google Assistant in Chrome OS except that it's all black 😉.

![G Assist Screenshot](images/Screenshot.png)
_(Google Assistant Unofficial Desktop Client Screenshot)_

## Getting Started

In order to use the client, you must have a _"Key File"_ and _"Token"_ for authentication which you can get by going through **Device Registration** process.

If you want a user friendly registration method, use Device Registration UI:
> https://developers.google.com/assistant/sdk/guides/library/python/embed/config-dev-project-and-account

If you want to use a CLI tool to complete the registration process manually, read the following:
> https://developers.google.com/assistant/sdk/reference/device-registration/register-device-manual

After you have registered your device and downloaded the required authentication files, you can head on to _Settings_ and set the _"Key File Path"_ and _"Saved Tokens Path"_ to the location where the respective files are located.

## How to Build?

```bash
# Get dependencies from npm
npm install

# Run the Assistant
npm start

# Build the Assistant (yarn recommended)
yarn dist
```

## Keyboard Shortcut

* **Windows:** Win + Shift + A
* **MacOS:** Cmd + Shift + A
* **Linux:** Super + Shift + A

## TODO

- [ ] Set `build` for Mac and Linux in _package.json_
- [x] Prompt user to install 'sox'
- [x] Create Config File
- [x] Remove 'auth' from the `app` folder
- [ ] Respond to "Ok Google" or "Hey Google"
- [x] Activate Mic for `continuousConverstion` only when audio output is done
- [x] Use different dependency for audio recording
- [ ] Improve Carousel UI Rendering in the `main_area`
- [x] Improve Error Handling
- [x] Improve Assistant Audio Output
- [x] Git
- [x] Turn off `webAudio` after visualization
- [x] "Enable Audio Output" in Settings
- [x] Divide Settings into sections
- [x] Don't accept empty queries
- [x] Info on each Setting
- [x] Animation while talking
- [x] Ping when activating mic
- [x] Welcome screen for first-time users
- [ ] Display images from Google Images
- [x] Option to disable auto-scaling

## Other Libraries Used

* **p5.js:** 
  * For visualization purpose when the user speaks through mic.
  * Link: https://p5js.org/

* **player.js:**
  * For playing audio through speakers.
  * Link: https://github.com/ItsWendell/google-assistant-desktop-client/blob/develop/src/renderer/providers/assistant/player.js
