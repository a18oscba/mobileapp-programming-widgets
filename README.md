I started of by creating a Linear Layout in the activity_main.xml file which looked something like.
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout 
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:visibility="visible"
    android:background="@android:color/darker_gray"
    tools:context=".MainActivity">
```
The first widget I wanted to add was a progress bar, for it to look good in my eyes I decided to center it and lengthen the width which looks more appealing. I started pushing with margins on the side but was happy with the results from "center". The only margin I was left with was from top to lower it down a little bit. The code looks like the following.

```
<ProgressBar
        android:id="@+id/progressBar"
        style="?android:attr/progressBarStyleHorizontal"
        android:layout_width="295dp"
        android:layout_height="50px"
        android:layout_gravity="center"
        android:layout_marginTop="50dp"
        android:progressBackgroundTint="#EE0000"
        android:progress="50"
        />
  ```
The second widget I wanted to add was a switch. There wasn't much new to this one I centered it as well and did a margin top because I didn't look good when it was too close to the progeress bar. The code looks like the following.
```
<Switch
        android:id="@+id/switch1"
        android:layout_width="230dp"
        android:layout_height="48dp"
        android:layout_gravity="center"
        android:layout_marginTop="25dp"
        android:layout_marginRight="35dp"
        android:text="Free WiFi" />
```

Lastly I added two checkboxes which I moved manually by margins this time instead of centering. Also added distance between the two for it to look better to the human eye. The code for both checkboxes looks like the following. Changed color and style as well.

```
<CheckBox
        android:id="@+id/checkBox"
        android:layout_width="241dp"
        android:layout_height="wrap_content"
        android:layout_marginLeft="50dp"
        android:layout_marginTop="35dp"
        android:buttonTint="@android:color/holo_green_light"

        android:text="Programmer"
        android:textAppearance="@style/TextAppearance.AppCompat.Body2" />

    <CheckBox
        android:id="@+id/checkBox2"
        android:layout_width="241dp"
        android:layout_height="wrap_content"
        android:layout_marginLeft="50dp"
        android:layout_marginTop="7dp"
        android:buttonTint="@android:color/holo_red_light"
        android:checked="false"
        android:clickable="true"
        android:text="UX Designer"
        android:textAppearance="@style/TextAppearance.AppCompat.Body2" />
```
