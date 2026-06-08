# UniChat 💬

**UniChat** é uma plataforma de comunicação moderna desenvolvida em Flutter e FastAPI, projetada especificamente para o ambiente universitário. O sistema permite que estudantes e professores interajam em tempo real, compartilhem informações e colaborem em projetos acadêmicos.

## Funcionalidades Principais

- **Mensagens em Tempo Real**: Comunicação instantânea com entrega garantida via WebSockets.
- **Grupos Acadêmicos**: Criação de salas de bate-papo dedicadas para turmas, projetos ou assuntos específicos.
- **Gerenciamento de Usuários**: Autenticação segura e perfis personalizados.
- **Interface Intuitiva**: Design limpo e responsivo desenvolvido com **Flutter**.
- **API Robusta**: Backend implementado em **FastAPI** para alta performance.
- **Conexão Professor-Aluno**: Ferramentas dedicadas para comunicação entre docentes e discentes.

---

## Tecnologias Utilizadas

### Frontend
- **[Flutter](https://flutter.dev/)**: Framework SDK para desenvolvimento de interfaces de usuário multiplataforma (Android, iOS, Web, Desktop).
- **Dart**: Linguagem de programação orientada a objetos.
- **Provider**: Gerenciamento de estado.
- **Socket.IO Client**: Cliente para comunicação em tempo real com o backend.

### Backend
- **[FastAPI](https://fastapi.tiangolo.com/)**: Framework web moderno para Python, baseado em type hints.
- **Python 3.10+**: Linguagem de programação.
- **[Socket.IO](https://socket.io/)**: Biblioteca para comunicação em tempo real.
- **Uvicorn/Gunicorn**: Servidores ASGI para execução do FastAPI.

---

## Estrutura do Projeto

O projeto é dividido em duas partes principais:

```
UniChat/
├── flutter_app/          # Aplicação Cliente (Frontend)
├── fastapi_app/          # API e Servidor de Tempo (Backend)
└── README.md             # Documentação Principal
```

### 1. flutter_app/
Contém todo o código da interface do usuário.
- `lib/`: Código fonte em Dart.
- `lib/screens/`: Telas da aplicação (Login, Chat, Grupos).
- `lib/models/`: Modelos de dados (Usuário, Mensagem, Grupo).
- `pubspec.yaml`: Dependências do Flutter.

### 2. fastapi_app/
Contém o backend e lógica de negócios.
- `main.py`: Ponto de entrada da API e servidor WebSocket.
- `services/`:
    - `time_sync_service.py`: Implementação do Algoritmo de Berkeley (Mestre).
    - `user_service.py`: Gerenciamento de usuários e salas.
- `schemas/`: Definições de schemas de dados (Pydantic).
- `requirements.txt`: Dependências do Python.
