
# E‑Chamados – Sistema de Chamados em PHP Nativo 🔧

Sistema simples de gerenciamento de chamados, feito em PHP puro, com foco em registrar solicitações, alterar status e visualizar o histórico de atendimento.

---

## 🔍 Sumário

- [Visão Geral](#visão-geral)  
- [Funcionalidades](#funcionalidades)  
- [Tecnologias Utilizadas](#tecnologias-utilizadas)  
- [Instalação e Configuração](#instalação-e-configuração)  
- [Uso](#uso)  
- [Estrutura do Projeto](#estrutura-do-projeto)  
- [Contribuição](#contribuição)  
- [Licença](#licença)

---

## 🎯 Visão Geral

O **E‑Chamados** é um sistema básico de atendimento para registrar, gerenciar e acompanhar chamados de suporte. É ideal para pequenas equipes ou uso educacional, com arquitetura minimalista e execução local ou em servidor PHP.

---

## ✅ Funcionalidades

- CRUD completo de chamados (criar, visualizar, editar, excluir).  
- Atribuição de status e responsáveis.  
- Histórico de alterações por chamado.  
- Painel de consulta com filtragem por status, prioridade e responsável.  
- Interface simples e funcional usando HTML e CSS nativo.

---

## 🛠️ Tecnologias Utilizadas

- **PHP 7+** – linguagem backend  
- **MySQL/MariaDB** – banco de dados (via PDO)  
- **HTML5 + CSS3** – front‑end limpo e responsivo  
- **JavaScript (vanilla)** – interatividade mínima (como validações)

---

## ⚙️ Instalação e Configuração

1. Clone o repositório:
   ```bash
   git clone https://github.com/sandoelio/E-Chamados.git
   ```
2. Acesse o diretório do projeto:
   ```bash
   cd E-Chamados
   ```
3. Configure o banco de dados:
   - Crie um banco (ex.: `echamados`)
   - Importe o arquivo SQL (ex.: `CREATE TABLE chamados (…)`)
4. Ajuste o arquivo `config.php` com suas credenciais de conexão:
   ```php
   $pdo = new PDO('mysql:host=localhost;dbname=echamados;charset=utf8', 'usuario', 'senha');
   ```
5. Copie para o seu servidor PHP (local ou remoto) e acesse via navegador:
   ```
   http://localhost/E-Chamados/index.php
   ```

---

## 🚀 Como Usar

- **Registrar um chamado**: preencha formulário com título, descrição, prioridade e atribua responsável.  
- **Visualizar chamados**: na lista principal, utilize filtros para status, prioridade ou responsável.  
- **Editar ou encerrar chamados**: altere status, responsável ou adicione observações.  
- **Excluir chamados**: remova registros antigos conforme necessário.

---

## 📂 Estrutura do Projeto

```
├── config.php      – Configuração de conexão com o banco
├── index.php       – Listagem e filtros de chamados
├── novo.php        – Formulário para criar novo chamado
├── editar.php      – Formulário para editar chamado
├── excluir.php     – Lógica de remoção
├── sql/            – Scripts para criação da tabela e populamento
└── assets/
    ├── css/        – Arquivos de estilo
    └── js/         – Scripts customizados (validação, modais etc.)
```

---

## 🤝 Contribuição

Contribuições são bem-vindas! Para colaborar:

1. Faça fork do repositório.  
2. Crie uma branch com sua feature (`git checkout -b feature/minha-feature`).  
3. Comite suas mudanças (`git commit -m 'Adicionar feature X'`).  
4. Envie (`git push origin feature/minha-feature`).  
5. Abra um Pull Request explicando o que foi alterado.

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para detalhes completos.

---

### 📝 Contato

Criado por **sandoelio**. Para melhorias, dúvidas ou sugestões, abra uma *issue* ou entre em contato!
