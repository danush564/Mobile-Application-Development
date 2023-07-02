# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Studio and then click on File -> New -> New project.
Step 2: Then type the Application name as HelloWorld and click Next. 
Step 3: Then select the Minimum SDK as shown below and click Next. 
Step 4: Then select the Empty Activity and click Next. Finally click Finish. 
Step 5: Design layout in activity_main.xml.
Step 6: Display message give in MainActivity file.
Step 7: Save and run the application.



## PROGRAM:
```
activity_main.xml :
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayoutxmlns:android="http://schemas.android.com/apk/res/android"
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
</androidx.constraintlayout.widget.ConstraintLayout>
option.xml :
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
<item android:title="Item 1" />
<item android:title="Item 2" />
<item android:title="Item 3" />
</menu>
MainActivity.java :
package com.example.menuoption;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;
public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);
    }
    @Override
    public booleanonCreateOptionsMenu(Menu menu) {
MenuInflater m = getMenuInflater();
m.inflate(R.menu.option,menu);
        return true;
    }
}

/*
Program to print the text “optionmenu”.
Developed by: DANUSH
Registeration Number : 212221040033
*/
```

## OUTPUT

![image](https://github.com/danush564/Mobile-Application-Development/assets/98585166/3b87e104-6fe0-430c-a4ee-f94dc2bf8de7)


![image](https://github.com/danush564/Mobile-Application-Development/assets/98585166/86f8ea65-fdaf-4e01-bbec-746a28c94b0e)


![image](https://github.com/danush564/Mobile-Application-Development/assets/98585166/035e3237-5a2e-43ea-9ba4-52e8fe496a59)


## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.


