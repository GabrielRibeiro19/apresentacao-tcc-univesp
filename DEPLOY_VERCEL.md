# 🚀 Como Fazer Deploy na Vercel

## Opção 1: Via Interface Web (Mais Fácil)

### Passo 1: Criar conta na Vercel
1. Acesse: https://vercel.com
2. Faça login com GitHub, GitLab ou email
3. É gratuito e não precisa de cartão de crédito

### Passo 2: Fazer Upload do Projeto
1. No dashboard da Vercel, clique em **"Add New..."** → **"Project"**
2. Escolha a opção **"Import Git Repository"** OU **"Deploy"** → **"Upload a folder"**
3. Se usar Git:
   - Conecte seu repositório (GitHub/GitLab/Bitbucket)
   - A Vercel detectará automaticamente os arquivos
4. Se usar Upload:
   - Arraste a pasta do projeto ou selecione os arquivos
   - Certifique-se de incluir:
     - `apresentacao.html`
     - `logo-univesp.png`
     - `fundo.jpg`
     - `figura-1.png`, `figura-2.png`, `fgura-3.png`, `figura-4.png`, `figura-5.png`
     - `apendice.jpg`

### Passo 3: Configurações
1. **Project Name**: Dê um nome ao projeto (ex: "tcc-apresentacao")
2. **Framework Preset**: Selecione **"Other"** ou **"Static"**
3. **Root Directory**: Deixe em branco ou coloque `./`
4. **Build Command**: Deixe em branco (não precisa de build)
5. **Output Directory**: Deixe em branco

### Passo 4: Deploy
1. Clique em **"Deploy"**
2. Aguarde alguns segundos
3. Pronto! Você receberá uma URL como: `https://seu-projeto.vercel.app`

### Passo 5: URLs Amigáveis
Após o deploy, você terá:
- **Apresentação principal**: `https://seu-projeto.vercel.app/` ou `https://seu-projeto.vercel.app/apresentacao`
- **Roteiro**: `https://seu-projeto.vercel.app/roteiro`

O arquivo `vercel.json` já está configurado para criar essas URLs amigáveis!

---

## Opção 2: Via CLI (Linha de Comando)

### Instalação da CLI
```bash
npm i -g vercel
```

### Login
```bash
vercel login
```

### Deploy
```bash
# No diretório do projeto
vercel

# Para produção
vercel --prod
```

### Deploy com arquivo específico
```bash
vercel apresentacao.html
```

---

## Opção 3: Renomear para index.html (Recomendado)

A forma mais simples é renomear o arquivo:

1. Renomeie `apresentacao.html` para `index.html`
2. Faça upload do projeto na Vercel
3. A página será exibida automaticamente como página inicial

---

## ✅ Checklist Antes do Deploy

- [ ] Todos os arquivos de imagem estão na mesma pasta:
  - [ ] `logo-univesp.png`
  - [ ] `fundo.jpg`
  - [ ] `figura-1.png`
  - [ ] `figura-2.png`
  - [ ] `fgura-3.png`
  - [ ] `figura-4.png`
  - [ ] `figura-5.png`
  - [ ] `apendice.jpg`
- [ ] Arquivo HTML principal (`index.html` - já renomeado)
- [ ] `roteiro_apresentacao.html` incluído
- [ ] `vercel.json` incluído (para URLs amigáveis)
- [ ] Testar localmente abrindo o HTML no navegador

---

## 🔧 Solução de Problemas

### Imagens não aparecem
- Verifique se todos os arquivos de imagem estão na mesma pasta do HTML
- Confirme que os nomes dos arquivos estão corretos (case-sensitive)

### Página não carrega
- Verifique se renomeou para `index.html` ou configurou o `vercel.json`
- Certifique-se de que o arquivo está na raiz do projeto

### URL personalizada
- Na Vercel, vá em **Settings** → **Domains**
- Você pode adicionar um domínio personalizado

---

## 📱 Acessar Durante a Apresentação

### Apresentação Principal:
1. Abra a URL: `https://seu-projeto.vercel.app/`
2. Pressione **F11** para tela cheia
3. Use as setas do teclado para navegar
4. Clique no botão "📋 Ver Roteiro" no canto inferior direito para abrir o roteiro

### Roteiro (para consulta em segundo plano):
1. Abra a URL: `https://seu-projeto.vercel.app/roteiro`
2. Cada pessoa pode abrir em seu dispositivo pessoal
3. Consulte discretamente durante a apresentação

---

## 💡 Dicas

- A Vercel é **gratuita** para projetos pessoais
- Deploy é **instantâneo** após fazer upload
- O projeto fica **online 24/7**
- Você pode fazer **deploys ilimitados**
- Cada deploy gera uma nova URL (pode manter versões antigas)

---

**Boa sorte na apresentação! 🎓**
