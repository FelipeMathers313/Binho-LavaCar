# Binho-LavaCar
Protótipo de aplicativo Android para agendamento e controle - Binho Lava Car
git init
git add .
git commit -m "Initial commit - protótipo Binho Lava Car"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/binho-lava-car.git
git push -u origin main
binho-lava-car/
├─ README.md
├─ LICENSE
├─ app/
│  ├─ src/
│  │  └─ main/
│  │     ├─ java/com/seudominio/binholavacar/
│  │     │   └─ MainActivity.kt
│  │     └─ res/
│  │        ├─ layout/activity_main.xml
│  │        └─ values/strings.xml
├─ prototype/
│  └─ figma-export.png
├─ docs/
│  └─ testes.md
└─ .gitignore# Binho Lava Car

Protótipo de um aplicativo Android para gerenciamento de agendamentos e controle de clientes do Lava Car "Binho". Desenvolvido como parte de projeto de extensão / prática acadêmica.

## Funcionalidades (protótipo)
- Cadastro básico de clientes
- Agendamento de serviços (hora/data)
- Notificações de lembrete (ex.: 30 minutos antes)
- Visualização da agenda do dia

## Tecnologias
- Android / Kotlin
- Android Studio (gradle)
- Banco de dados local (SQLite) ou Firebase (opcional)

## Estrutura do repositório
- `app/` — código-fonte Android (Kotlin)
- `prototype/` — protótipos de telas (imagens)
- `docs/` — documentação de testes e evidências

## Como executar (versão local)
1. Abra o Android Studio.
2. Importe o módulo `app/`.
3. Rode em um emulador ou dispositivo Android.

## Evidências e testes
As pastas `docs/` e `prototype/` contêm capturas de tela, prints de testes, logs e notas de usabilidade que documentam o desenvolvimento e a verificação do protótipo.

---

> Projeto criado para fins acadêmicos e de demonstração. Para contato: fel-tof@hotmail.com
> *.iml
.gradle/
local.properties
/.idea
/build
/captures
.externalNativeBuild
package com.seudominio.binholavacar

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import android.widget.Button
import android.widget.Toast

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        val btnSample: Button = findViewById(R.id.btnSample)
        btnSample.setOnClickListener {
            Toast.makeText(this, "Protótipo: agendamento criado (exemplo)", Toast.LENGTH_SHORT).show()
        }
    }
}<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical" android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="24dp">

    <TextView
        android:id="@+id/tvTitle"
        android:text="Binho Lava Car - Protótipo"
        android:textSize="20sp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"/>

    <Button
        android:id="@+id/btnSample"
        android:layout_marginTop="20dp"
        android:text="Criar agendamento (teste)"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"/>
</LinearLayout>


