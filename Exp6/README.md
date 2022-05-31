# Ex.No: 6 Build a program to create a first display screen of any search engine using Auto Complete Text View.

## AIM:

To develop a program to create a first display screen of any search engine using AutoComplete TextView in Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min.required Arctic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as "searchengine" and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout using AutoComplete TextView in activity_main.xml.

Step 6: Display screen of search engine in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to “display screen of any search engine”.
Developed by        : Marinto Richee J
Registration Number : 212220230031
*/
```
### MainActivity.java
```
package com.example.auto_complete_view_experiment;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.ArrayAdapter;
import android.widget.AutoCompleteTextView;

public class MainActivity extends AppCompatActivity {
    AutoCompleteTextView autocomplete;

    String[] arr = { "Bing","Google","Yandex","Yahoo","DuckDuckGo","Swisscows","StartPage","Gibiru"};

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        autocomplete = (AutoCompleteTextView)
                findViewById(R.id.autoCompleteTextView1);

        ArrayAdapter<String> adapter = new ArrayAdapter<String>
                (this,android.R.layout.select_dialog_item, arr);

        autocomplete.setThreshold(2);
        autocomplete.setAdapter(adapter);
    }
}
```
### activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#A86D6D"
    android:padding="5dp"
    tools:context=".MainActivity">


    <AutoCompleteTextView
        android:id="@+id/autoCompleteTextView1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/textView2"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="30dp"
        android:layout_marginTop="30dp"
        android:layout_marginEnd="30dp"
        android:layout_marginBottom="30dp"
        android:ems="10"
        android:hint="@string/example_autocompletetextview"
        android:textAlignment="center"
        tools:ignore="UnknownId" />

</RelativeLayout>
```

## OUTPUT:

![1](https://user-images.githubusercontent.com/65499285/169662709-a51e1efa-e4ae-4112-8167-c441f7ea2ea5.png)

![2](https://user-images.githubusercontent.com/65499285/169662712-0e935f8b-2791-4f65-a71f-ed1cbbae9753.png)

![3](https://user-images.githubusercontent.com/65499285/169662713-cb6c8fec-2d9f-4c5a-8c2d-3f521b2ade29.png)

![4](https://user-images.githubusercontent.com/65499285/169662715-e1fcd6ed-3cf5-45e1-9ae4-3634a0d08275.png)

![5](https://user-images.githubusercontent.com/65499285/169662716-c67c5a54-f47b-41e8-8965-a3c651427d55.png)

## RESULT:
Thus a Simple Android Application to create a first display screen of any search engine using AutoComplete TextView in Android Studio is developed and executed successfully.
