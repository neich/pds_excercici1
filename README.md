# PDS Exercici 1 - Plantilla Android

Plantilla base per als exercicis de l'assignatura de **Projecte de desenvolupament de software (PDS) a la UdG**.

## 📋 Requisits

- **Android Studio Ladybug** o superior
- **JDK 11**
- **SDK Android 36** (mínim SDK 29)

## 🚀 Començar

1. Clona o descarrega el projecte
2. Obre'l amb Android Studio
3. Sincronitza Gradle (`File > Sync Project with Gradle Files`)
4. Executa l'aplicació en un emulador o dispositiu físic

## 📁 Estructura del projecte

```
app/src/main/
├── java/com/example/myapplication/
│   └── MainActivity.java       ← Activitat principal
├── res/
│   └── layout/
│       └── activity_main.xml   ← Layout principal
└── AndroidManifest.xml
```

## ✨ Característiques incloses

| Característica | Descripció |
|----------------|------------|
| **View Binding** | Accés tipat a les vistes del layout |
| **Navigation SafeArgs** | Pas de paràmetres segur entre fragments |
| **Edge-to-Edge** | Suport per a pantalla completa |
| **Material Design 3** | Components de UI moderns |

## 🔧 View Binding

El projecte utilitza View Binding per accedir a les vistes:

```java
// El binding es genera automàticament a partir del layout XML
ActivityMainBinding binding = ActivityMainBinding.inflate(getLayoutInflater());
setContentView(binding.getRoot());

// Accedeix a les vistes directament
binding.textView.setText("Hola!");
```

## 📦 Dependències principals

Les versions estan centralitzades a `gradle/libs.versions.toml`:

- AndroidX AppCompat
- Material Components
- Navigation (Fragment + UI)
- ConstraintLayout

## ⚠️ Notes importants

- **Package**: `com.example.myapplication` - Canvia'l si cal pel teu exercici
- **Namespace**: Definit a `app/build.gradle`
- **minSdk**: 29 (Android 10)

---
*Plantilla per a PDS - Curs 2025-2026*

