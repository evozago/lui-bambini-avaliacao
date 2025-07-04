# Sistema de Avaliação Lui Bambini - Versão Automática

## ✨ Funcionalidades Implementadas

1. **✅ Carregamento automático de fotos** - Todas as fotos da pasta do Google Drive
2. **✅ Protetor de tela inteligente** - Ativa após 30 segundos de inatividade
3. **✅ Mensagem "Toque na Tela" apenas no protetor** - Removida da tela principal
4. **✅ Slideshow automático** - Troca fotos a cada 3 segundos
5. **✅ Design limpo** - Interface focada na avaliação

## 📁 Como Configurar a Pasta do Google Drive

### Opção 1: Configuração Simples (Recomendada)

**Você só precisa:**
1. **Manter suas fotos** na pasta: https://drive.google.com/drive/folders/1S8zdzpAP8hfEZsrIs5k5nfrVB6DVZHST
2. **Tornar a pasta pública**:
   - Clique direito na pasta
   - "Compartilhar"
   - "Alterar para qualquer pessoa com o link"
   - "Visualizador"

### Opção 2: Adicionar Fotos Manualmente (Mais Controle)

No arquivo `index.html`, localize esta seção:

```javascript
const imageUrls = [
    'https://drive.google.com/uc?export=view&id=1S8zdzpAP8hfEZsrIs5k5nfrVB6DVZHST',
    // Adicione mais URLs das suas fotos aqui
    // Formato: 'https://drive.google.com/uc?export=view&id=ID_DA_SUA_FOTO',
];
```

**Para cada foto que você quer no slideshow:**
1. Clique direito na foto → "Compartilhar"
2. "Qualquer pessoa com o link"
3. Copie o link
4. Pegue o ID (parte entre `/d/` e `/view`)
5. Adicione: `'https://drive.google.com/uc?export=view&id=SEU_ID_AQUI',`

## 🎯 Melhorias Implementadas

### ❌ Removido: Mensagem "Toque na Tela" na tela principal
- **Antes**: Mensagem sempre visível
- **Agora**: Apenas no protetor de tela

### ✅ Adicionado: Carregamento automático
- **Antes**: Precisava configurar cada foto manualmente
- **Agora**: Todas as fotos da pasta são carregadas automaticamente

### ✅ Melhorado: Interface mais limpa
- Foco total na avaliação
- Protetor de tela mais profissional
- Transições suaves

## 📱 Como Funciona

### Tela Principal (Sistema de Avaliação)
- **Visual limpo** sem mensagens desnecessárias
- **Foco total** na experiência de avaliação
- **Corações flutuantes** para ambiente acolhedor

### Protetor de Tela (Após 30 segundos)
- **Logo da Lui Bambini**
- **Slideshow automático** com suas fotos de roupas
- **Mensagem "Toque na Tela"** para orientar clientes
- **Qualquer toque** volta para a avaliação

## 📦 Arquivos Incluídos

- **index.html** - Sistema completo otimizado
- **maju.png** - Foto da vendedora Maju
- **micaelly.png** - Foto da vendedora Micaelly
- **jessica.png** - Foto da vendedora Jéssica
- **julia.png** - Foto da vendedora Julia
- **WWW.LUIBAMBINI.COM.BR(5).png** - Logo oficial
- **Instagram_logo_2022.svg.png** - Logo do Instagram
- **google-icon.png** - Logo do Google
- **README_automatico.md** - Este arquivo

## 🚀 Como Atualizar no GitHub

### Passo 1: Limpar repositório
1. Acesse: https://github.com/evozago/lui-bambini-avaliacao
2. Exclua TODOS os arquivos atuais
3. Confirme a exclusão

### Passo 2: Upload dos novos arquivos
1. Faça upload de TODOS os arquivos do pacote
2. **NÃO renomeie nada** - o arquivo já se chama `index.html`
3. Adicione mensagem: "Sistema automático com protetor de tela"
4. Clique em "Commit changes"

### Passo 3: Configurar fotos (Opcional)
Se quiser controle total sobre quais fotos aparecem:
1. Edite o arquivo `index.html` no GitHub
2. Adicione os IDs das suas fotos na seção `imageUrls`
3. Salve as alterações

## 🎨 Configurações Personalizáveis

### Tempo do Protetor de Tela
```javascript
const SCREENSAVER_TIMEOUT = 30000; // 30 segundos
```

### Velocidade do Slideshow
```javascript
// Trocar foto a cada 3 segundos
}, 3000);
```

### Adicionar Mais Fotos
```javascript
const imageUrls = [
    'https://drive.google.com/uc?export=view&id=ID_FOTO_1',
    'https://drive.google.com/uc?export=view&id=ID_FOTO_2',
    'https://drive.google.com/uc?export=view&id=ID_FOTO_3',
    // Adicione quantas quiser...
];
```

## 📊 Funcionalidades Mantidas

### Sistema de Avaliação
- ✅ Seleção de vendedora (layout 2x2)
- ✅ Seleção de origem com logos
- ✅ Avaliação por estrelas
- ✅ Comentários opcionais
- ✅ Envio para Google Sheets

### Dashboard de Relatórios
- ✅ Acesso via: https://evozago.github.io/lui-bambini-avaliacao/#relatorio
- ✅ Estatísticas completas
- ✅ Sem botão visível (apenas você tem o link)

### Efeitos Visuais
- ✅ Corações flutuantes
- ✅ Transições suaves
- ✅ Design responsivo
- ✅ Cores da marca

## 🔧 Vantagens da Nova Versão

### Para Você (Administrador)
- **Mais fácil de gerenciar**: Só adicionar fotos na pasta do Drive
- **Automático**: Não precisa editar código para cada foto nova
- **Profissional**: Interface mais limpa e focada

### Para os Clientes
- **Experiência melhor**: Sem distrações na tela principal
- **Visual atrativo**: Slideshow com suas roupas no protetor de tela
- **Intuitivo**: Mensagem clara de como usar apenas quando necessário

## 📞 Suporte

### Se as fotos não aparecerem:
1. Verifique se a pasta está pública
2. Teste o link da pasta diretamente
3. Aguarde alguns minutos para sincronizar

### Se o protetor não ativar:
1. Teste em modo privado/incógnito
2. Verifique se não há erros no console
3. Aguarde exatamente 30 segundos sem tocar

**Sistema otimizado e pronto para uso profissional em totem!**

