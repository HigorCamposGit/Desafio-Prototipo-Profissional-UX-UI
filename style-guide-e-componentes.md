# 02. Design System & Style Guide

Este documento define as diretrizes visuais, tokens de design e componentes reutilizáveis aplicados no Figma para garantir consistência, acessibilidade e escalabilidade.

---

## 1. Paleta de Cores

A escolha cromática utiliza tons quentes (vermelho terracota e laranja âmbar) para estimular o apetite e destacar chamadas para ação (CTAs), equilibrados por superfícies neutras claras para leitura confortável do cardápio.

| Categoria | Token | Hexadecimal | Uso na Interface |
| :--- | :--- | :--- | :--- |
| **Primária** | `color-primary-500` | `#D9381E` | Botões principais (CTAs), preço em destaque, ícones ativos |
| **Primária Hover** | `color-primary-700` | `#A8240F` | Estado pressionado / foco de botões |
| **Secundária** | `color-secondary-500` | `#F59E0B` | Badges de avaliação (estrelas), tags de promoção e pontos |
| **Fundo Principal** | `color-bg-canvas` | `#F9FAFB` | Fundo geral das telas do aplicativo |
| **Superfície / Cards**| `color-bg-surface` | `#FFFFFF` | Fundo dos cards de pratos, modais e barra de navegação |
| **Texto Principal** | `color-text-primary` | `#1F2937` | Títulos de pratos, cabeçalhos e valores principais |
| **Texto Secundário** | `color-text-secondary`| `#6B7280` | Descrições de ingredientes, tempo estimado e subtítulos |
| **Sucesso** | `color-feedback-success`| `#10B981` | Status "Pedido Entregue", confirmação de Pix e frete grátis |
| **Erro / Alerta** | `color-feedback-error` | `#EF4444` | Campos obrigatórios inválidos e remoção de item |

---

## 2. Tipografia

* **Família Tipográfica:** `Plus Jakarta Sans` (Títulos) e `Inter` (Corpo de texto e interfaces — excelente legibilidade em telas pequenas).

| Estilo | Fonte | Peso | Tamanho | Line-Height | Uso |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **H1 (Título Tela)** | Plus Jakarta Sans | Bold (700) | `24px` | `32px` | Saudação na Home, título do Checkout |
| **H2 (Seção)** | Plus Jakarta Sans | SemiBold (600)| `18px` | `24px` | Categorias ("Pratos Executivos", "Bebidas") |
| **Subtitle / Card** | Inter | SemiBold (600)| `16px` | `22px` | Nome do prato no card |
| **Body Regular** | Inter | Regular (400) | `14px` | `20px` | Descrição dos ingredientes |
| **Caption / Badge** | Inter | Medium (500) | `12px` | `16px` | Tempo de entrega, tags e labels |
| **Button Label** | Inter | SemiBold (600)| `15px` | `20px` | Texto interno dos botões de ação |

---

## 3. Grid e Espaçamento (Sistema 8pt)

* **Frame Mobile:** `390 x 844 px`
* **Grid de Layout:** 4 colunas, margem lateral de `16px`, gutter (espaçamento entre colunas) de `16px`.
* **Escala de Espaçamento:** Múltiplos de `4px` e `8px` (`4px`, `8px`, `12px`, `16px`, `24px`, `32px`).
* **Border Radius (Arredondamento):**
  * Cards de produtos e inputs: `12px`
  * Botões principais: `10px`
  * Badges e chips de categoria: `999px` (formato pílula)

---

## 4. Componentes Padronizados (Figma Auto Layout)

1. **Botão Primário (`btn-primary`):** Altura `48px`, fundo `#D9381E`, texto `#FFFFFF`, raio `10px`, estados: *Default*, *Pressed* e *Disabled*.
2. **Card de Prato Horizontal (`card-dish`):** Foto quadrada à esquerda (`88x88px`, raio `8px`), título, descrição limitada a 2 linhas, tempo de preparo e preço em negrito à direita.
3. **Chips de Categoria (`chip-category`):** Lista horizontal com estados *Ativo* (fundo `#D9381E`, texto branco) e *Inativo* (fundo `#FFFFFF`, borda `#E5E7EB`).
4. **Seletor de Quantidade (`stepper-qty`):** Botões `-` e `+` com contador centralizado e área de toque mínima de `36x36px`.
5. **Barra de Navegação Inferior (`bottom-nav`):** Fixa na base (`72px` de altura) com 4 itens: *Início*, *Busca*, *Pedidos* e *Perfil*.