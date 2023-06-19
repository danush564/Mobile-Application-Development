# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by:DANUSH S
Registeration Number :212221040033
*/
activity_main.xml :
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout
xmlns:android="http://schemas.android.com/apk/res/android"
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
app:layout_constraintEnd_toEndOf="parent"
app:layout_constraintStart_toStartOf="parent"
app:layout_constraintTop_toTopOf="parent" />
</android.support.constraint.ConstraintLayout>

MainActivity.java :
/*
Program to print the text “Hello World”.
Developed by: DANUSH S
Registration Number: 212221040033
*/
package com.example.exp1; import android.os.Bundle;
import android.support.v7.app.AppCompatActivity;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
@Override
protected void onCreate(Bundle savedInstanceState) {
   super.onCreate(savedInstanceState);
   setContentView(R.layout.activity_main);
   Toast.makeText(this, "onCreate Called", Toast.LENGTH_SHORT).show();
}
@Override
protected void onRestart(){
   Toast.makeText(this, "onRestart Called", Toast.LENGTH_SHORT).show();
   super.onRestart();
}
@Override
protected void onStart(){
   Toast.makeText(this, "onStart Called", Toast.LENGTH_SHORT).show();
   super.onStart();
}
@Override
protected void onResume(){
   Toast.makeText(this, "onResume Called", Toast.LENGTH_SHORT).show();
   super.onResume();
}
@Override
protected void onPause(){
   Toast.makeText(this, "onPause Called", Toast.LENGTH_SHORT).show();
   super.onPause();
}
@Override
protected void onStop(){
   Toast.makeText(this, "onStop Called", Toast.LENGTH_SHORT).show();
   super.onStop();
}
@Override
protected void onDestroy(){
   Toast.makeText(this, "onDestroy Called", Toast.LENGTH_SHORT).show();
   super.onDestroy();
}
}


## OUTPUT

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/98585166/6a1ff5bb-eb9a-49e6-81e3-e5d20f763c8e)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/98585166/a287b5dd-bd0d-485a-a122-b290319637e5)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/98585166/6ae44aad-2a0d-4b66-8ba0-821ac1e032e9)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/98585166/15a32842-b649-480c-8237-824832775289)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/98585166/08c6141b-b3b1-40ae-bb71-e0d465f106b2)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
