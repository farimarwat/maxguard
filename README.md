# MaxGuard
An android library for android app security agains reverse engineering

MaxGuard is a maximum security layer to protect against reverse engineering via frida. This library tries to detect frida injection and close the app if injection is found.

### What is frida
Frida is a super powerful tool to inject android apps to extract sensitive data. It can defeat any kind of encryption even AES. So to secure android app, it is most important
to detect frida injection.

## Setup

### Implementation
```
    implementation("io.github.farimarwat:maxguard:1.1")
```

### Usabe
```
override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        MaxGuard()
            .startMaxGuard()
}
```
