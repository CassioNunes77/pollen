# Pollen - Site Oficial

Site moderno e responsivo para a plataforma Pollen, desenvolvido com HTML, CSS e JavaScript puro.

## 🚀 Características

- **Design Moderno**: Interface minimalista e sofisticada com glassmorphism
- **Totalmente Responsivo**: Adaptado para todos os dispositivos
- **Animações Suaves**: GSAP para animações de scroll e interações
- **Efeitos Visuais**: Gradientes animados, paralaxe e partículas WebGL (opcional)
- **Performance**: Carregamento otimizado e lazy loading
- **Acessibilidade**: Navegação por teclado, contraste adequado e semântica HTML

## 🎨 Paleta de Cores

O site utiliza uma paleta de cores escura com acentos vibrantes:

- **Fundo Principal**: `#0a0a0f` (Preto escuro)
- **Fundo Secundário**: `#111118` (Cinza muito escuro)
- **Acento Primário**: `#8B5CF6` (Lilás)
- **Acento Secundário**: `#3B82F6` (Azul neon)

As cores podem ser facilmente customizadas através das variáveis CSS em `styles.css`.

## 📁 Estrutura de Arquivos

```
pollen-1/
├── index.html          # Página principal (landing page)
├── privacy.html        # Página de políticas de privacidade
├── styles.css          # Estilos principais
├── main.js             # JavaScript principal
├── README.md           # Este arquivo
├── netlify.toml        # Configuração Netlify
└── .nojekyll           # Arquivo para GitHub Pages
```

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica
- **CSS3**: Variáveis CSS, Grid, Flexbox, Glassmorphism
- **JavaScript ES6**: Módulos modernos
- **GSAP**: Animações e scroll triggers
- **Three.js**: Efeito de partículas WebGL (opcional, desabilitado em mobile)
- **Lottie**: Suporte para animações vetoriais (preparado)

## 📦 Dependências (CDN)

O site utiliza CDNs para as seguintes bibliotecas:

- **GSAP 3.12.2**: Animações
- **ScrollTrigger**: Plugin GSAP para scroll
- **Three.js r128**: Efeitos WebGL
- **Lottie 5.12.2**: Animações vetoriais
- **Google Fonts**: Inter e Space Grotesk

## 🚀 Deploy

### GitHub Pages

1. Faça push do código para um repositório GitHub
2. Vá em Settings > Pages
3. Selecione a branch `main` (ou `master`)
4. Selecione a pasta `/ (root)`
5. Clique em Save

O site estará disponível em: `https://seu-usuario.github.io/pollen-1/`

**Nota**: O arquivo `.nojekyll` garante que o GitHub Pages não processe o site com Jekyll.

### Netlify

#### Opção 1: Deploy via Git

1. Conecte seu repositório GitHub ao Netlify
2. Configure:
   - **Build command**: (deixe vazio)
   - **Publish directory**: `/` (raiz)
3. Clique em "Deploy site"

#### Opção 2: Deploy Manual

1. Instale o Netlify CLI:
   ```bash
   npm install -g netlify-cli
   ```

2. Faça login:
   ```bash
   netlify login
   ```

3. Deploy:
   ```bash
   netlify deploy --prod
   ```

O arquivo `netlify.toml` já está configurado com as opções corretas.

## 🎯 Funcionalidades

### Navegação
- Menu responsivo com animação
- Scroll suave entre seções
- Navegação por teclado (acessibilidade)

### Animações
- **Hero**: Título e subtítulo com fade-in sequencial
- **Scroll Reveals**: Elementos aparecem ao rolar a página
- **Hover Effects**: Microinterações em cards e botões
- **Paralaxe**: Efeito sutil em backgrounds
- **Partículas WebGL**: Campo de partículas no hero (desabilitado em mobile)

### Seções
1. **Hero**: Apresentação principal com CTA
2. **Features**: Grid de recursos com ícones SVG
3. **Portfolio**: Showcase de projetos
4. **Testimonials**: Depoimentos de clientes
5. **CTA**: Formulário de contato
6. **Footer**: Links e informações

## 🎨 Customização

### Cores

Edite as variáveis CSS em `styles.css`:

```css
:root {
    --color-bg-primary: #0a0a0f;
    --color-accent-primary: #8B5CF6;
    --color-accent-secondary: #3B82F6;
    /* ... */
}
```

### Fontes

As fontes podem ser alteradas nas variáveis:

```css
:root {
    --font-primary: 'Inter', sans-serif;
    --font-display: 'Space Grotesk', sans-serif;
}
```

### Animações

Para desabilitar animações (acessibilidade), o CSS já inclui:

```css
@media (prefers-reduced-motion: reduce) {
    /* Animações desabilitadas */
}
```

## 📱 Responsividade

O site é totalmente responsivo com breakpoints:

- **Desktop**: > 768px
- **Tablet**: 768px - 1024px
- **Mobile**: < 768px

## ♿ Acessibilidade

- Navegação por teclado
- Contraste adequado (WCAG AA)
- Textos semânticos
- ARIA labels onde necessário
- Suporte a `prefers-reduced-motion`

## 🔧 Desenvolvimento Local

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/pollen-1.git
   cd pollen-1
   ```

2. Abra `index.html` em um navegador ou use um servidor local:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Node.js (com http-server)
   npx http-server
   ```

3. Acesse: `http://localhost:8000`

## 📝 Notas

- O efeito WebGL (partículas) é automaticamente desabilitado em dispositivos móveis para melhor performance
- As animações GSAP têm fallback para Intersection Observer caso a biblioteca não carregue
- Imagens podem ser adicionadas usando lazy loading com `data-src`

## 📄 Licença

Este projeto é propriedade da Pollen. Todos os direitos reservados.

## 🤝 Contribuindo

Para contribuições, por favor abra uma issue ou pull request.

---

Desenvolvido com ❤️ para Pollen

