package com.example.primeraapp;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.TextView;

public class ThirdActivity extends AppCompatActivity {
    TextView Dato;
    String Valor;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_third);
        Dato = findViewById(R.id.Dato);
        Bundle extras = getIntent().getExtras();
        Valor = extras.getString("Valor");
        Dato.setText(Valor);

    }
}
