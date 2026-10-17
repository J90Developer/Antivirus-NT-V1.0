Antivirus NT V1.0/
├── docs/                               # Documentación técnica
├── shared/                             # Interoperabilidad entre componentes
│   ├── proto/ipc_messages.proto        # Mensajes IPC estructurados en Protocol Buffers
│   └── rules/eicar.yar                 # Regla YARA estándar para pruebas EICAR
├── src/
│   ├── engine/                         # Motor nativo C++20 (CMakeLists.txt + vcpkg.json)
│   │   ├── include/sentinel/           # Headers públicos (core, scanner, heuristics, quarantine, ipc)
│   │   ├── src/                        # Implementación interna
│   │   └── tests/                      # Suite GoogleTest
│   ├── client-desktop/                 # Aplicación C# .NET 8 WPF / MVVM
│   │   ├── src/ (App, Core, IPC)
│   │   └── tests/
│   ├── backend-cloud/                  # Microservicio Java 21 / Spring Boot 3 (pom.xml)
│   └── web-dashboard/                  # Consola Web (HTML5, CSS3 dark-mode, app.js)
├── scripts/
│   └── build-all.ps1                   # Script de verificación y compilación
├── .gitignore
├── ARCHITECTURE.md
├── SECURITY.md
├── ROADMAP.md
├── TESTING.md
└── README.md
