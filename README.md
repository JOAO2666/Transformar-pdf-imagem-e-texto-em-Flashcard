# 🧠 Transformar PDF, Imagem e Texto em Flashcards para Anki

Um gerador inteligente de flashcards que utiliza IA (Gemini) para converter conteúdo de PDF, imagens e texto em flashcards prontos para importar no Anki.

## 🌟 Funcionalidades

- **📄 Suporte a múltiplos formatos**: PDF, imagens (PNG, JPG, JPEG) e texto simples
- **🤖 IA integrada**: Utiliza o Google Gemini para gerar flashcards inteligentes
- **👁️ OCR avançado**: Extração de texto de imagens usando Tesseract.js
- **✏️ Edição em tempo real**: Edite as perguntas e respostas diretamente na interface
- **📥 Exportação para Anki**: Exporta diretamente no formato CSV compatível com Anki
- **📱 Interface responsiva**: Funciona perfeitamente em desktop e mobile
- **🎨 Design moderno**: Interface elegante com tema escuro

## 🚀 Demo ao Vivo

Acesse a aplicação: [Gemini](https://g.co/gemini/share/470ccae87ebd)

## 🛠️ Como Usar

1. **Faça upload do arquivo**: Arraste e solte ou clique para selecionar um arquivo PDF, imagem ou texto
2. **Gere os flashcards**: Clique em "Gerar Flashcards com IA" e aguarde o processamento
3. **Revise e edite**: Modifique as perguntas e respostas conforme necessário
4. **Exporte para o Anki**: Baixe o arquivo CSV e importe no seu Anki

## 📋 Pré-requisitos

Para usar a aplicação, você precisará de:

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexão com a internet (para a IA processar o conteúdo)
- Anki instalado (para importar os flashcards gerados)

## 🔧 Configuração Local

### Clone o repositório
```bash
git clone https://github.com/JOAO2666/Transformar-pdf-imagem-e-texto-em-Flashcard.git
cd Transformar-pdf-imagem-e-texto-em-Flashcard
```

### Configuração da API
Para usar localmente, você precisará configurar uma chave da API do Google Gemini:

1. Vá para [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Crie uma nova chave API
3. Substitua a variável `apiKey` no arquivo `index.html` pela sua chave

### Execução Local
Como é uma aplicação puramente frontend, você pode:

1. **Servidor HTTP simples com Python:**
```bash
python -m http.server 8000
```

2. **Servidor HTTP simples com Node.js:**
```bash
npx http-server
```

3. **Ou simplesmente abrir o arquivo `index.html` no navegador**

## 🌐 Deploy no Netlify

### Opção 1: Conectar Repositório GitHub
1. Acesse [Netlify](https://netlify.com)
2. Clique em "New site from Git"
3. Conecte seu repositório GitHub
4. O deploy será automático!

### Opção 2: Deploy Manual
1. Faça upload da pasta do projeto diretamente no Netlify
2. O site estará disponível instantaneamente

### Configuração de Variáveis de Ambiente (Opcional)
Para maior segurança, você pode configurar a chave da API como variável de ambiente no Netlify:

1. Vá em Site Settings > Environment Variables
2. Adicione `GEMINI_API_KEY` com sua chave
3. Modifique o código para usar `process.env.GEMINI_API_KEY`

## 📁 Estrutura do Projeto

```
Transformar-pdf-imagem-e-texto-em-Flashcard/
│
├── index.html          # Arquivo principal da aplicação
├── README.md           # Este arquivo
└── netlify.toml        # Configurações do Netlify (opcional)
```

## 🔗 Tecnologias Utilizadas

- **HTML5/CSS3/JavaScript**: Base da aplicação
- **TailwindCSS**: Framework CSS para estilização
- **PDF.js**: Biblioteca para leitura de arquivos PDF
- **Tesseract.js**: OCR para extração de texto de imagens
- **Google Gemini API**: IA para geração inteligente de flashcards
- **Inter Font**: Tipografia moderna

## 📖 Como Importar no Anki

1. Abra o Anki
2. Vá em `File > Import`
3. Selecione o arquivo CSV baixado
4. Configure:
   - **Field separator**: Semicolon
   - **Field 1**: Front
   - **Field 2**: Back
5. Clique em `Import`

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 🐛 Reportar Bugs

Encontrou um bug? [Abra uma issue](https://github.com/JOAO2666/Transformar-pdf-imagem-e-texto-em-Flashcard/issues) descrevendo:

- Qual navegador você está usando
- Qual tipo de arquivo estava processando
- Passos para reproduzir o problema
- Mensagem de erro (se houver)

## 💡 Melhorias Futuras

- [ ] Suporte a mais formatos de arquivo (DOCX, EPUB)
- [ ] Diferentes tipos de flashcards (múltipla escolha, verdadeiro/falso)
- [ ] Salvamento local de flashcards
- [ ] Integração direta com Anki Connect
- [ ] Suporte a múltiplos idiomas
- [ ] Temas personalizáveis

## 👨‍💻 Autor

**João** - [GitHub](https://github.com/JOAO2666)

---

⭐ **Se este projeto foi útil para você, considere dar uma estrela!** 
