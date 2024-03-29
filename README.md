# Teste Prático: Sistema de Cotação para Tradução com OCR e Dados do Cliente

## Objetivo
Desenvolver uma aplicação web que permita aos usuários fazer upload de fotos de documentos para extração de texto via OCR, selecionar idiomas de origem e destino, e obter uma cotação para o serviço de tradução. Os usuários também devem fornecer suas informações de contato, incluindo nome, e-mail e número de WhatsApp, este último com uma máscara de entrada adequada.

## Funcionalidades Detalhadas

### Formulário de Informações do Usuário
- Incluir campos para o usuário inserir seu **nome**, **e-mail** e **número de WhatsApp**.
- Implementar validações para garantir que os dados inseridos estão no formato correto.

### Máscara de Entrada para o WhatsApp
- Aplicar uma máscara de entrada no campo do WhatsApp para formatar automaticamente os números de telefone conforme o padrão internacional.
- A máscara deve ser flexível para acomodar diferentes formatos de números de telefone de países ao redor do mundo.

### Upload e Análise de Documentos
- Permitir que os usuários façam upload de imagens de documentos.
- Utilizar OCR para extrair o texto das imagens.
- Contar o número de palavras do texto extraído.

### Cálculo e Exibição de Preço
- Após a contagem de palavras, multiplicar o número total pelo preço por palavra, que deve ser definido como:
  - Para traduções de Italiano: R$ 0,25 por palavra.
  - Para traduções de Inglês: R$ 0,20 por palavra.
- Exibir o preço estimado na tela para o usuário.

### Armazenamento de Dados
- Armazenar informações sobre cada pedido, incluindo dados do usuário, detalhes do documento e cotação, no banco de dados.

## Requisitos Técnicos Adicionais

- **Validação de Dados:** Garantir que todos os campos do formulário sejam validados adequadamente.

## Desafios de Implementação

- **Interface de Usuário Intuitiva:** Criar uma interface clara e fácil de usar, orientando o usuário através do processo de forma intuitiva. PS. Design não será avaliado
- **Flexibilidade da Máscara de Entrada:** Implementar uma máscara de entrada para o WhatsApp que aceite e formate números de diferentes países.
- **Extração de texto usando OCR:** Utilizar uma biblioteca ou API de OCR (como Tesseract, Google Cloud Vision API, Amazon Textract ou similar) para extrair texto de imagens de documentos enviados pelos usuários.


## Stack do projeto

- PHP >= 8.0 (Se quiser usar Laravel não tem problema)
- MySQL
- jQuery/Ajax
- HTML/CSS (Se quiser pode usar Bootstrap ou Tailwind)
- Ambientalização com Docker
  
Os requisitos de front-end não são obrigatórios, pode desenvolver no que se sentir mais confortável e produtivo.

**Importante: O projeto deve seguir a arquitetura MVC.**

---
