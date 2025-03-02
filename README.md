# 🏆 **Desafio Técnico – Laravel 12 + Livewire + Tailwind CSS**

## 🎯 **Objetivo**
Criar uma aplicação web utilizando **Laravel 12, Livewire e Tailwind CSS** que permita aos usuários:
- Fazer **upload de imagens de documentos** para extração de texto via **OCR**.
- Selecionar **idiomas de origem e destino** para cotação de tradução.
- **Calcular e exibir um preço estimado** baseado no número de palavras extraídas.
- **Armazenar os pedidos** no banco de dados.

---

## 📌 **Requisitos Técnicos**
### 🔹 **Stack do projeto**
- Laravel **12** com **Livewire**
- Tailwind CSS
- PostgreSQL ou MySQL
- Laravel Herd ou Docker (para desenvolvimento local)
- Biblioteca de OCR (Google Cloud Vision ou Amazon Textract)
- Máscara para telefone usando **[International Telephone Input](https://intl-tel-input.com/)**

---

## 📝 **Funcionalidades**
### 🔹 **Formulário de Informações do Usuário**
- Campos obrigatórios:
  - **Nome**
  - **E-mail**
  - **Número de WhatsApp** (com máscara)
- **Validações**:
  - Nome: obrigatório
  - E-mail: obrigatório e válido
  - WhatsApp: obrigatório e formatado corretamente
- **Seleção de idiomas de origem e destino**:
  - Opções: **Português, Inglês, Italiano**.
  - **Regra**: O usuário **sempre** deve selecionar **Português** como um dos idiomas (ex.: **Português → Inglês**, **Português → Italiano**).

---

### 🔹 **Upload e OCR**
- **Upload via Livewire**
- Arquivos aceitos: **PNG, JPG, PDF, DOC, DOCX, XLS, XLSX**
- Após o envio:
  - Aplicar **OCR** para extrair o texto do documento.
  - Contar **número de palavras** do texto extraído.

---

### 🔹 **Cálculo do Preço da Tradução**
- Preço por palavra:
  - **Inglês:** R$ 0,20
  - **Italiano:** R$ 0,25
- Exibir dinamicamente o valor total baseado no número de palavras extraídas.

---

### 🔹 **Armazenamento no Banco de Dados**
- Criar **migration** para armazenar:
  - Nome, e-mail, WhatsApp.
  - Idioma de origem e destino.
  - Caminho do arquivo enviado.
  - Texto extraído pelo OCR.
  - Número de palavras e valor calculado.

---

## 🚀 **Desafios Extras (Diferencial)**
✅ Criar **notificação via e-mail** com o resumo do pedido.  
✅ Permitir **upload direto para S3, Cloud Storage ou R2** (Livewire suporta isso).  
✅ Melhorar a interface com **Livewire Loading States** para feedback ao usuário.  
✅ Utilizar instalação do Laravel com startkit Livewire  
✅ Usar [FluxUI](https://fluxui.dev/) para a UI do formulário

---

## 📌 **Critérios de Avaliação**
🔹 Código limpo e bem estruturado seguindo o **MVC**  
🔹 Uso correto de **Livewire** para interatividade sem recarregar a página  
🔹 **Validações backend e frontend** bem implementadas  
🔹 Organização e boas práticas do Laravel  
🔹 Uso de **Eloquent** para interação com o banco  

---

## 🔥 **Como Entregar**
- Enviar o código pelo **GitHub** (repositório público ou privado com acesso).

---

🎯 **Objetivo do teste**: Avaliar sua capacidade de trabalhar com **Laravel 12, Livewire, Tailwind**, interações assíncronas e boas práticas de desenvolvimento.

🔹 **Boa sorte!** 🚀

---
