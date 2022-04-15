# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as “ex.no.1″ and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: Marinto Richee J
Registeration Number : 212220230031
*/
```
### MainActivity.java:
```
package com.example.exno1;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}
```
### activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## OUTPUT:
<img width="945" alt="image_2022-04-09_18-47-45" src="https://user-images.githubusercontent.com/65499285/162582462-29fa07df-2ecf-4f47-83e8-0d6ffa75b0c1.png">
<img width="947" alt="image_2022-04-09_18-48-31" src="https://user-images.githubusercontent.com/65499285/162582484-c587dead-ed1e-41da-a0df-8c37d586ef24.png">
<img width="945" alt="image_2022-04-09_18-49-48" src="https://user-images.githubusercontent.com/65499285/162582503-43a0e877-1ce7-48f5-8ef8-5c85e49e5e93.png">
<img width="946" alt="image_2022-04-09_18-50-04" src="https://user-images.githubusercontent.com/65499285/162582509-ce0e263e-5a56-4ff9-ba78-79af115f2285.png">
<img width="944" alt="image_2022-04-09_18-50-35" src="https://user-images.githubusercontent.com/65499285/162582516-cf8edc0c-91f1-4423-9014-698ed83cf80d.png">
<img width="947" alt="image_2022-04-09_18-50-54" src="https://user-images.githubusercontent.com/65499285/162582520-6d4ec024-2d52-4824-8645-f623d404b3dd.png">
<img width="945" alt="image_2022-04-09_18-51-48" src="https://user-images.githubusercontent.com/65499285/162582527-f5bd77d2-9861-45d3-808b-fc887cc0007e.png">

## RESULT:
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
