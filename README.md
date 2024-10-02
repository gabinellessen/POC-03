```markdown
# POC-03: Media Queries no CSS
### Resumo:
Essa POC tem como explicar como usar usar forma plena a media queries. Iremos explicar as funcionalidades principais da característca do CSS que é tão importante para navegabilidade em mobile. 
## 1. Media Query para Impressão

As media queries para **impressão** permitem definir estilos específicos que serão aplicados apenas quando a página for impressa. Isso garante que o conteúdo seja apresentado de forma clara e legível no papel.

```css
@media print {
  body {
    font-size: 12pt;
    color: black;
  }
  .no-print {
    display: none;
  }
}
```

### Explicação:
- **`font-size: 12pt`**: Ajusta o tamanho da fonte para 12 pontos, um tamanho padrão para impressão.
- **`color: black`**: Garante que o texto seja impresso em preto, independentemente das cores usadas na tela.
- **`display: none`**: Oculta elementos que não são necessários na versão impressa, como menus de navegação.

## 2. Media Queries para Diferentes Larguras de Dispositivos

As media queries para diferentes **larguras de dispositivos** permitem a criação de layouts responsivos que se adaptam a diferentes tamanhos de tela, como smartphones, tablets e desktops.

Exemplos:

```css
@media (max-width: 768px) {
  /* Estilos aplicados para dispositivos com largura de até 768px (tablets) */
}

@media (max-width: 480px) {
  /* Estilos aplicados para dispositivos com largura de até 480px (smartphones) */
}
```

### Explicação:
- **`max-width: 768px`**: Aplica estilos para dispositivos com largura de até 768 pixels (tablets).
- **`max-width: 480px`**: Aplica estilos para dispositivos com largura de até 480 pixels (smartphones).

## 3. Media Queries para Orientação de Dispositivos

As media queries para **orientação** permitem ajustar o layout com base na posição do dispositivo, seja em modo paisagem (landscape) ou retrato (portrait).

Exemplos:

```css
@media (orientation: portrait) {
  /* Estilos aplicados quando o dispositivo está em modo retrato */
}

@media (orientation: landscape) {
  /* Estilos aplicados quando o dispositivo está em modo paisagem */
}
```

### Explicação:
- **`orientation: portrait`**: Aplica estilos quando o dispositivo está em modo retrato.
- **`orientation: landscape`**: Aplica estilos quando o dispositivo está em modo paisagem.

## 4. Outras Propriedades Importantes de Media Queries

Outras propriedades que podem ser úteis ao trabalhar com **media queries**:

- **`column-count`**: Define o número de colunas para o texto.
- **`column-gap`**: Define o espaçamento entre as colunas.
- **`max-width: 992px`**: Aplica estilos para dispositivos com largura de até 992 pixels (ideal para tablets).
- **`max-width: 600px`**: Aplica estilos para dispositivos com largura de até 600 pixels (ideal para smartphones).

