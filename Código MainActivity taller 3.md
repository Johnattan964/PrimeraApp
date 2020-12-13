<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:visibility="visible"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/signup"
        android:layout_width="355dp"
        android:layout_height="43dp"
        android:layout_marginBottom="32dp"
        android:text="Sign Up"
        android:textColor="@color/black"
        app:backgroundTint="@color/white"
        app:layout_constraintBottom_toTopOf="@+id/policy"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:strokeColor="@color/blue" />

    <Button
        android:id="@+id/login"
        android:layout_width="355dp"
        android:layout_height="43dp"
        android:layout_marginBottom="12dp"
        android:text="Login"
        android:textColor="@color/white"
        app:backgroundTint="@color/blue"
        app:layout_constraintBottom_toTopOf="@+id/signup"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:strokeColor="@color/red" />


    <EditText
        android:id="@+id/password"
        android:layout_width="350dp"
        android:layout_height="45dp"
        android:layout_marginTop="10dp"
        android:ems="10"
        android:hint="Password"
        android:inputType="textPassword"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.54"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/name" />

    <CheckBox
        android:id="@+id/remember"
        android:layout_width="148dp"
        android:layout_height="29dp"
        android:layout_marginStart="32dp"
        android:layout_marginTop="50dp"
        android:layout_marginBottom="164dp"
        android:shadowColor="@color/black"
        android:text="Remember me"
        android:visibility="visible"
        app:layout_constraintBottom_toTopOf="@+id/login"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/password"
        app:layout_constraintVertical_bias="0.333" />

    <TextView
        android:id="@+id/recuperation"
        android:layout_width="wrap_content"
        android:layout_height="28dp"
        android:layout_marginTop="50dp"
        android:layout_marginEnd="34dp"
        android:layout_marginBottom="164dp"
        android:bufferType="normal"
        android:gravity="center|center_horizontal|center_vertical"
        android:text="Forgot Password"
        app:layout_constraintBottom_toTopOf="@+id/login"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toEndOf="@+id/remember"
        app:layout_constraintTop_toBottomOf="@+id/password"
        app:layout_constraintVertical_bias="0.375" />

    <TextView
        android:id="@+id/policy"
        android:layout_width="235dp"
        android:layout_height="0dp"
        android:layout_marginBottom="36dp"
        android:gravity="center|center_horizontal|center_vertical"
        android:text="Term of use. Privacy Policy "
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />

    <EditText
        android:id="@+id/name"
        android:layout_width="350dp"
        android:layout_height="45dp"
        android:layout_marginTop="20dp"
        android:ems="10"
        android:hint="Useername"
        android:inputType="textPersonName"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.54"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/logo" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintGuide_begin="20dp" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintGuide_begin="20dp" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        app:layout_constraintGuide_begin="20dp" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline4"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        app:layout_constraintGuide_begin="20dp" />

    <ImageView
        android:id="@+id/logo"
        android:layout_width="150dp"
        android:layout_height="150dp"
        android:layout_marginTop="20dp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        android:src="@drawable/unirem"/>

</androidx.constraintlayout.widget.ConstraintLayout>
