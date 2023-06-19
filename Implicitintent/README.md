# Ex.No:3 Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the google page using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Studio and then click on File -> New -> New project.
Step 2: Then type the Application name as HelloWorld and click Next. 
Step 3: Then select the Minimum SDK as shown below and click Next. 
Step 4: Then select the Empty Activity and click Next. Finally click Finish. 
Step 5: Design layout in activity_main.xml
Step 6: Display message give in MainActivity file.
Step 7: Save and run the application.


## PROGRAM:
activity_main.xml :
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent"
android:background="@color/purple_200" 
tools:context=".MainActivity">
<Button android:id="@+id/button"
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_marginEnd="48dp" 
android:text="NAVIGATE"
app:layout_constraintBottom_toBottomOf="parent" 
app:layout_constraintEnd_toEndOf="parent" 
app:layout_constraintTop_toTopOf="parent" 
app:layout_constraintVertical_bias="0.219" />
<EditText
android:id="@+id/editTextTextPersonName" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_marginStart="32dp" 
android:ems="10"
android:inputType="textPersonName" 
app:layout_constraintBottom_toBottomOf="parent" 
app:layout_constraintStart_toStartOf="parent" 
app:layout_constraintTop_toTopOf="parent" 
app:layout_constraintVertical_bias="0.218" />
</android.support.constraint.ConstraintLayout>
MainActivity.java :
/*
Program to print the text “Implicitintent”. 
Developed by:DANUSH S
Registration Number: 212221040033
*/
package com.example.intent;
import android.support.v7.app.AppCompatActivity; 
import android.os.Bundle;
import android.content.Intent; 
import android.net.Uri;
import android.widget.Button; 
import android.widget.EditText;

public class MainActivity extends AppCompatActivity {
    Button button;
    EditText editText;
    @Override
    protected void onCreate(Bundle savedInstanceState) { 
     super.onCreate(savedInstanceState);
     setContentView(R.layout.activity_main); 
     button = findViewById(R.id.button);
     editText = findViewById(R.id.editTextTextPersonName); 
     button.setOnClickListener(view -> {
      String url=editText.getText().toString();
      Intent intent=new Intent(Intent.ACTION_VIEW, Uri.parse(url)); 
      startActivity(intent);
});
}
}

## OUTPUT
![image](https://github.com/danush564/Mobile-Application-Development/assets/98585166/c987b675-847e-4f52-ac7f-c7b8c64c6392)
![image](https://github.com/danush564/Mobile-Application-Development/assets/98585166/92e9d9d1-6fde-4a00-bb6e-f999f18a3dc9)
![image](https://github.com/danush564/Mobile-Application-Development/assets/98585166/3d69543d-7982-411e-b014-bf973f1ae7cb)



## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the google page using Android Studio is developed and executed successfully.


