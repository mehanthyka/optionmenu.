# Ex.No:10 To create a option menu to display menu items.
### AIM:
To create a option menu to display menu items.
### EQUIPMENTS REQUIRED:
Latest Version Android Studio

### ALGORITHM:
Step 1: Open Android Studio and then click on File -> New -> New project. 
<br>Step 2: Then type the Application name as “option menu” and click Next.
<br>Step 3: Then select the Minimum SDK as shown below and click Next.
<br>Step 4: Then select the Empty Activity and click Next. Finally click Finish. 
<br>Step 5: Design layout in activity_main.xml.
<br>Step 6: Get contacts details and Display details give in MainActivity file.
<br>Step 7: Save and run the application..

### PROGRAM:
~~~
/*
Program to print the text “optionmenu”.
Developed by:Mehanthyka D
Registeration Number :212221040105
*/
~~~
### activity_main.xml
~~~
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
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
~~~
### MainActivity.java
~~~
package com.example.optionmenu;
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
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.option,menu);
        return true;
    }
}
option.xml
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="Item 1" />
    <item android:title="Item 2" />
    <item android:title="Item 3" />
</menu>
~~~
      
### OUTPUT
![image](https://github.com/mehanthyka/optionmenu./assets/127507580/8fc6439e-c12c-4a26-aeae-b81c1325a05a)
![image](https://github.com/mehanthyka/optionmenu./assets/127507580/22888f51-943b-4445-921d-e67685c673bc)
![image](https://github.com/mehanthyka/optionmenu./assets/127507580/7800c634-8482-4d46-a820-fd41f884e9ea)
![image](https://github.com/mehanthyka/optionmenu./assets/127507580/b747e18d-ae93-475f-96e6-6461b4f75943)

### RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
