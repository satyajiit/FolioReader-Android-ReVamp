![FolioReader logo](https://raw.githubusercontent.com/FolioReader/FolioReaderKit/assets/folioreader.png)

[![Build Status](https://api.travis-ci.org/FolioReader/FolioReader-Android.svg?branch=master)](https://travis-ci.org/FolioReader/FolioReader-Android)

FolioReader-Android is an EPUB reader written in Java and Kotlin. ( Forked, Fixed Bugs and ReVamped UI )

### Features

- [x] Custom Fonts
- [x] Custom Text Size
- [x] Themes / Day mode / Night mode
- [x] Text Highlighting
- [x] List / Edit / Delete Highlights
- [x] Handle Internal and External Links
- [x] Portrait / Landscape
- [ ] Reading Time Left / Pages left
- [x] In-App Dictionary
- [ ] Media Overlays (Sync text rendering with audio playback)
- [ ] TTS - Text to Speech Support
- [ ] Parse epub cover image
- [ ] PDF support
- [x] Book Search
- [x] Add Notes to a Highlight
- [ ] Better Documentation
- [x] Last Read Locator
- [x] Horizontal Reading
- [x] Distraction Free Reading

## Demo
##### Custom Fonts
![Custom fonts](https://cloud.githubusercontent.com/assets/1277242/19012915/0661c7b2-87e0-11e6-81d6-8c71051e1074.gif)
##### Day and Night Mode
![Day night mode](https://cloud.githubusercontent.com/assets/1277242/19012914/f42059c4-87df-11e6-97f8-29e61a79e8aa.gif)
##### Text Highlighting
![Highlight](https://cloud.githubusercontent.com/assets/1277242/19012904/c2700c3a-87df-11e6-97ed-507765b3ddf0.gif)
##### Media Overlays
![Media Overlay](https://cloud.githubusercontent.com/assets/1277242/19012908/d61f3ce2-87df-11e6-8652-d72b6a1ad9a3.gif)

### Gradle

Add following dependency to your root project `build.gradle` file:

```groovy
allprojects {
    repositories {
        ...
        jcenter()
        maven { url "https://jitpack.io" }
        ...
    }
}
```

Add following dependency to your app module `build.gradle` file:

```groovy
dependencies {
    ...
    implementation 'com.github.satyajiit:FolioReader-Android-ReVamp:v0.4'
    ...
}
```

### Enable Multidex support

Enable Multidex support as explained in this [Android Doc](https://developer.android.com/studio/build/multidex)

### Usage

Get singleton object of `FolioReader`:

```java
FolioReader folioReader = FolioReader.get();
```

Call the function `openBook()`:

##### opening book from assets -

```java
folioReader.openBook("file:///android_asset/TheSilverChair.epub");
```
##### opening book from raw -

```java
folioReader.openBook(R.raw.accessible_epub_3);
```


## INFO

* This is forked version of [FolioReader-Android](https://github.com/FolioReader/FolioReader-Android)
* Made with Custom UI and fonts
* Fixed issue with fonts not being changed
* Multidex is not required for SDK > 21




## License
FolioReaderKit is available under the BSD license. See the [LICENSE](https://github.com/FolioReader/FolioReader-Android/blob/master/License.md) file.

