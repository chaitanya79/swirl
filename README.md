Swirl
======

A simple, animated icon to use when interacting with the fingerprint reader.

![](images/sample.gif)


Usage
-----

Swirl does not provide default colors, so you must specify them in your theme.

```xml
<style name="Theme.YourApp" parent="@android:style/Theme.Material.Light">
  <item name="swirl_ridgeColor">?android:attr/textColorSecondary</item>
  <item name="swirl_errorColor">?android:attr/colorAccent</item>
</style>
```

Then, you may include `SwirlView` anywhere in your app.

```xml
<com.mattprecious.swirl.SwirlView
    android:layout_width="60dp"
    android:layout_height="60dp"
    />
```

Note that this example specifies a width and height and does not use `wrap_content`. Swirl
uses vector drawables and does not have a default size, so you must specify one.

Switch between icons by calling `setState()` or by using the `app:swirl_state` attribute.

See the provided sample for a complete implementation.


Download
--------

Gradle:

```groovy
compile 'com.mattprecious.swirl:swirl:0.1.0'
```


License
--------

    Copyright 2016 Matthew Precious

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

