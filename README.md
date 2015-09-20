#### build.gradle
```java
    compile 'com.android.support:percent:23.0.1'
```

#### XML
```xml
<android.support.percent.PercentRelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_below="@id/appbar">

        <View
            android:id="@+id/view_left"
            android:layout_width="0dp"
            android:layout_height="0dp"
            android:background="#aa22dc"
            android:elevation="40dp"
            app:layout_heightPercent="20%"
            app:layout_widthPercent="70%" />

        <View
            android:id="@+id/view_right"
            android:layout_width="0dp"
            android:layout_height="0dp"
            android:layout_alignParentTop="true"
            android:layout_toRightOf="@+id/view_left"
            android:background="#da1f1f"
            android:elevation="40dp"
            app:layout_heightPercent="20%"
            app:layout_widthPercent="30%" />

        <View
            android:id="@+id/bottom"
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_below="@+id/view_left"
            android:background="#f7d113"
            app:layout_heightPercent="80%" />

    </android.support.percent.PercentRelativeLayout>
```