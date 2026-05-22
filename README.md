# 🎵 API Musiquinhas

A **API Musiquinhas** é uma interface simplificada e eficiente desenvolvida para o gerenciamento de catálogos musicais. Ela permite o cadastro, a listagem completa e a busca detalhada de faixas musicais de forma rápida e padronizada. Com esta API, desenvolvedores podem integrar facilmente recursos de organização de áudio e playlists em suas aplicações.

🌍 **URL Base de Produção:** `https://api.musiquinhas.com/v1`

---

## 📖 Documentação Integrada

A documentação interativa completa desta API (renderizada via Swagger/Redoc) está disponível publicamente através do GitHub Pages.

🔗 **Acesse aqui:** [Documentação Oficial no GitHub Pages](https://gustavoazzola76261-arch.github.io/minha-api/)

---

## 🚀 Endpoints Disponíveis

Abaixo estão listadas as rotas configuradas na API e suas respectivas funções:

### 🎼 Músicas (`/musica`)

#### `GET /musica`
* **Descrição:** Retorna a lista completa de todas as músicas cadastradas na plataforma.
* **Resposta de Sucesso:** `200 OK` (Retorna um array com as músicas).

#### `POST /musica`
* **Descrição:** Realiza o cadastro de uma nova música no catálogo.
* **Corpo da Requisição (JSON):**
  ```json
  {
    "titulo": "Minha musiquinhas"
  }

* **Respostas:**

201 Created: Música criada com sucesso.

400 Bad Request: Dados inválidos ou ausência do campo obrigatório titulo.

### `Detalhes (/Musica/{id})`
### `GET /Musica/{id}`
* **Descrição:** Busca e retorna as informações detalhadas de uma música específica utilizando o seu identificador (id) informado na URL.

* **Parâmetros:** id (string, obrigatório no caminho da URL).

* **Respostas:**

200 OK: Música localizada com sucesso.

404 Not Found: Nenhuma música foi encontrada com o ID fornecido.
