# Sistema de Avaliação Lui Bambini - Com Protetor de Tela

## ✨ Novas Funcionalidades Implementadas

1. **✅ Protetor de tela automático** - Ativa após 30 segundos de inatividade
2. **✅ Slideshow de fotos de roupas** - Carrega imagens do Google Drive
3. **✅ Mensagem "Toque na Tela"** - Fixa na parte inferior para orientar clientes
4. **✅ Detecção de atividade** - Qualquer toque/movimento sai do protetor de tela
5. **✅ Design responsivo** - Funciona perfeitamente em iPad e outros dispositivos

## 🖼️ Configuração das Imagens do Google Drive

### Passo 1: Preparar as imagens no Google Drive

1. **Acesse sua pasta**: https://drive.google.com/drive/folders/1S8zdzpAP8hfEZsrIs5k5nfrVB6DVZHST
2. **Para cada imagem que você quer no slideshow**:
   - Clique com o botão direito na imagem
   - Selecione "Compartilhar"
   - Clique em "Alterar para qualquer pessoa com o link"
   - Copie o ID da imagem (a parte entre `/d/` e `/view` na URL)

### Passo 2: Atualizar o código

No arquivo `index_com_drive.html`, localize esta seção:

```javascript
const imageUrls = [
    'https://drive.google.com/uc?export=view&id=SUBSTITUA_PELO_ID_DA_IMAGEM_1',
    'https://drive.google.com/uc?export=view&id=SUBSTITUA_PELO_ID_DA_IMAGEM_2',
    'https://drive.google.com/uc?export=view&id=SUBSTITUA_PELO_ID_DA_IMAGEM_3',
    'https://drive.google.com/uc?export=view&id=SUBSTITUA_PELO_ID_DA_IMAGEM_4',
    'https://drive.google.com/uc?export=view&id=SUBSTITUA_PELO_ID_DA_IMAGEM_5',
];
```

**Substitua cada `SUBSTITUA_PELO_ID_DA_IMAGEM_X` pelo ID real da sua imagem.**

### Exemplo prático:

Se sua imagem tem a URL:
`https://drive.google.com/file/d/1ABC123XYZ789/view?usp=sharing`

O ID é: `1ABC123XYZ789`

Então você colocaria:
`'https://drive.google.com/uc?export=view&id=1ABC123XYZ789',`

## 📱 Como Funciona o Protetor de Tela

### Ativação Automática
- **Tempo**: 30 segundos sem atividade
- **Detecção**: Mouse, toque, teclado, scroll
- **Visual**: Slideshow com fotos de roupas

### Conteúdo do Protetor de Tela
- **Logo da Lui Bambini** no topo
- **Texto**: "Lui Bambini - Moda Infantil com Amor"
- **Slideshow**: Fotos das roupas (troca a cada 3 segundos)
- **Call-to-action**: "Toque na tela para avaliar nosso atendimento"

### Saída do Protetor de Tela
- **Qualquer toque** na tela
- **Movimento do mouse**
- **Tecla pressionada**
- **Scroll** na página

## 🎯 Configuração para iPad (Totem)

### Configuração Inicial
1. Abra o Safari no iPad
2. Acesse: https://evozago.github.io/lui-bambini-avaliacao/
3. Toque no botão "Compartilhar" (quadrado com seta)
4. Selecione "Adicionar à Tela de Início"
5. Configure o iPad para não entrar em modo de espera

### Configurações Recomendadas do iPad
- **Brilho**: 80-90% para boa visibilidade
- **Modo de espera**: Desativado
- **Rotação**: Bloqueada em paisagem ou retrato
- **Notificações**: Desativadas para o Safari
- **Modo guiado**: Ativado para evitar saída acidental

## 📦 Arquivos Incluídos

- **index_com_drive.html** - Sistema completo com protetor de tela
- **maju.png** - Foto da vendedora Maju
- **micaelly.png** - Foto da vendedora Micaelly
- **jessica.png** - Foto da vendedora Jéssica
- **julia.png** - Foto da vendedora Julia
- **WWW.LUIBAMBINI.COM.BR(5).png** - Logo oficial da Lui Bambini
- **Instagram_logo_2022.svg.png** - Logo do Instagram
- **google-icon.png** - Logo do Google
- **README_screensaver.md** - Este arquivo com instruções

## 🚀 Como Atualizar no GitHub

### Passo 1: Limpar repositório atual
1. Acesse: https://github.com/evozago/lui-bambini-avaliacao
2. Exclua TODOS os arquivos atuais
3. Confirme a exclusão

### Passo 2: Upload dos novos arquivos
1. Faça upload de TODOS os arquivos do pacote
2. **IMPORTANTE**: Renomeie `index_com_drive.html` para `index.html`
3. Adicione uma mensagem como "Sistema com protetor de tela"
4. Clique em "Commit changes"

### Passo 3: Configurar as imagens
1. Edite o arquivo `index.html` no GitHub
2. Substitua os IDs das imagens pelos IDs reais do seu Google Drive
3. Salve as alterações

## 🎨 Personalização

### Tempo do Protetor de Tela
Para alterar o tempo de ativação (padrão: 30 segundos):
```javascript
const SCREENSAVER_TIMEOUT = 30000; // 30 segundos em milissegundos
```

### Velocidade do Slideshow
Para alterar a velocidade de troca das imagens (padrão: 3 segundos):
```javascript
// Trocar imagem a cada 3 segundos
slideshowTimer = setInterval(() => {
    // código...
}, 3000); // 3 segundos em milissegundos
```

### Cores e Estilo
As cores foram ajustadas para combinar com a identidade visual:
- **Gradiente principal**: #9acdbc (verde claro) para #4b72a2 (azul)
- **Cor de destaque**: #9acdbc (verde claro)
- **Botões**: Gradiente verde-azul

## 📊 Funcionalidades Mantidas

### Sistema de Avaliação
- Seleção de vendedora com fotos reais (layout 2x2)
- Seleção de origem com logos das empresas
- Avaliação por estrelas e comentários opcionais
- Envio automático para Google Sheets

### Dashboard de Relatórios
- **Acesso**: https://evozago.github.io/lui-bambini-avaliacao/#relatorio
- Estatísticas completas e gráficos
- Sem botão visível (apenas você tem o link)

### Mensagem "Toque na Tela"
- **Posição**: Fixa na parte inferior
- **Estilo**: Destaque com animação pulsante
- **Ícone**: 👆 para indicar ação de toque
- **Sempre visível**: Mesmo quando não está no protetor de tela

## 🔧 Solução de Problemas

### Se as imagens não carregarem:
1. Verifique se as imagens estão públicas no Google Drive
2. Confirme se os IDs estão corretos
3. Teste os links diretamente no navegador

### Se o protetor de tela não ativar:
1. Verifique se não há erros no console do navegador
2. Confirme se o tempo está configurado corretamente
3. Teste em modo privado/incógnito

### Se o toque não sair do protetor de tela:
1. Verifique se o iPad está em modo responsivo
2. Teste com diferentes tipos de toque
3. Reinicie o navegador se necessário

**Sistema completo com protetor de tela profissional para uso em totem!**

