package com.example.primeraapp;
import android.content.Intent;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.CheckBox;
import android.widget.EditText;
import android.widget.ImageView;
import android.widget.TextView;
import android.widget.Toast;

import java.nio.file.Files;
import java.util.Objects;

public class MainActivity extends AppCompatActivity {
    ImageView logo;
    Button signup, login;
    EditText password, name;
    CheckBox remenber;
    TextView recuperation, policy;
    String Nombre, Password;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        logo = findViewById(R.id.logo);
        password = findViewById(R.id.password);
        name = findViewById(R.id.name);
        signup = findViewById(R.id.signup);
        login = findViewById(R.id.login);
        recuperation = findViewById(R.id.recuperation);

        signup.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                Toast.makeText(getApplicationContext(),"Esta dando clik en registro", Toast.LENGTH_SHORT).show();

                            }
        });


        login.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                Nombre = name.getText().toString();
                Password = password.getText().toString();
            if(Objects.equals(Nombre, "Admin")& Objects.equals(Password, "1234")){
                    Intent intent = new Intent(MainActivity.this,ThirdActivity.class);
                    intent.putExtra("Valor",Nombre);
                    startActivity(intent);
            }else{
                   Toast.makeText(getApplicationContext(),"Datos incorrectos", Toast.LENGTH_SHORT).show();
                }



                //Toast.makeText(getApplicationContext(),"Click a Login", Toast.LENGTH_SHORT).show();
            }
        });




    }
}
