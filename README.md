# **CineBox - Plataforma Fullstack de Avaliação e Marcação de Filmes/Séries**
Aplicação web fullstack de catálogo de filmes/séries, onde permite o usuário navegar por filmes e séries por meio de APIs, avaliar e organizar suas séries e filmes favoritos/assistidos. A plataforma oferece funcionalidades completas para gerenciar o que você já assistiu, marcar favoritos para assistir depois e atribuir avaliações e opiniões pessoais.

## 📋 **Funcionalidades Principais**
- **Catálogo de Filmes e Séries**: Descubra títulos populares e busque informações detalhadas diretamente de APIs externas, como TMDb ou OMDb.
- **Favoritos**: Adicione filmes e séries à sua lista de favoritos para assistir mais tarde.
- **Assistidos**: Marque filmes/séries como assistidos e atribua uma avaliação por estrelas com opiniões personalizadas.
- **Autenticação**: Registro e login de usuários com segurança utilizando JWT.
- **Interface Responsiva**: Design moderno, acessível em dispositivos desktop e móveis.

---

## 🛠️ **Tecnologias Utilizadas**
### **Frontend**
- **React.js**: Biblioteca para construção da interface.
- **React Router**: Gerenciamento de rotas no frontend.
- **Fetch API**: Para integração com APIs (backend e externa).

### **Backend**
- **FastAPI**: Framework leve e eficiente para construção de APIs.
- **PyJWT**: Para autenticação segura via tokens JWT.
- **MongoDB**: Banco de dados NoSQL para armazenamento dos dados.

### **API Externa**
- **TMDb/OMDb**: Para buscar informações detalhadas sobre filmes e séries.

---

## 🚀 **Como Executar o Projeto**
### Pré-requisitos
- Node.js, Python 3.9+ e MongoDB instalados.

### Passos para rodar localmente:
1. **Clone o repositório**:
   ```bash
   git clone https://github.com/Sanmiir/catalogo-filmes.git
   cd catalogo-filmes
2. **Inicie o backend**:

   ```bash
   Copiar código
   cd backend
   python -m venv env
   source env/bin/activate       # Linux/Mac
   env\Scripts\activate          # Windows
   pip install -r requirements.txt
   uvicorn api.main:app --reload
   Inicie o frontend:
3. **Inicie o Frontend**:
   ```bash
   Copiar código
   cd frontend
   npm install
   npm start
   Certifique-se de que o MongoDB está rodando localmente ou configure o acesso remoto.

5. **Acesse a aplicação em**:

-**Frontend**: [http://localhost:3000](http://localhost:3000)
-**Backend**: [http://localhost:8000/docs](http://localhost:8000/docs) (Swagger UI para testar endpoints)

---

## 🗂️ **Estrutura do Projeto**
```bash
project-root/
├── frontend/
│   ├── src/
│   │   ├── components/   # Componentes reutilizáveis
│   │   ├── pages/        # Páginas da aplicação
│   │   ├── services/     # Lógica para consumir APIs
│   └── App.js            # Configuração de rotas
├── backend/
│   ├── api/
│   ├── models/           # Modelos para o banco de dados
│   ├── services/         # Lógica do backend e integração com API externa
│   └── database.py       # Conexão com MongoDB
└── README.md

---



