# 03. Wireframes, Arquitetura e Prototipagem

Este documento detalha a estrutura das telas projetadas no Figma, as decisões de usabilidade e a lógica de navegação interativa do protótipo de alta fidelidade.

---

## 1. Arquitetura das Telas (5 Telas Principais)

### Tela 01: Splash Screen / Boas-Vindas
* **Objetivo:** Apresentar a identidade visual da marca e direcionar o usuário ao cardápio sem barreiras de cadastro obrigatório imediato.
* **Elementos:** Logotipo *Sabor Brasileiro Express*, ilustração/foto de destaque, botão primário *"Ver Cardápio"* e link secundário *"Já tenho conta"*.

### Tela 02: Home / Cardápio Principal
* **Objetivo:** Permitir que o usuário encontre seu prato ou escolha o especial do dia em menos de 30 segundos.
* **Elementos:**
  * Cabeçalho com endereço de entrega selecionado e ícone de notificações.
  * Barra de busca rápida (*"Buscar prato, bebida..."*).
  * Banner promocional do **Prato do Dia** com botão direto de pedido.
  * Carrossel horizontal de categorias (*Todos*, *Executivos*, *Marmitas*, *Bebidas*, *Sobremesas*).
  * Lista vertical de cards de pratos com foto, descrição resumida, tempo estimado e preço.
  * Barra de navegação inferior fixa (*Início*, *Busca*, *Pedidos*, *Perfil*).

### Tela 03: Detalhes e Personalização do Prato
* **Objetivo:** Eliminar erros de cozinha permitindo escolhas claras antes de adicionar à sacola.
* **Elementos:**
  * Imagem expandida do prato no topo com botão flutuante de voltar.
  * Título, descrição completa dos ingredientes e valor unitário.
  * Seleção obrigatória (Radio Button) de acompanhamento principal (*Arroz e Feijão*, *Arroz Integral*, *Salada Mix*).
  * Seleção opcional (Checkbox) de adicionais (*Ovo Frito*, *Farofa Especial*, *Batata Frita*).
  * Campo de texto aberto para observações (*"Ex: Tirar cebola, mandar talheres"*).
  * Barra fixa inferior com seletor de quantidade (`- 1 +`) e botão *"Adicionar • R$ XX,XX"*.

### Tela 04: Sacola / Checkout
* **Objetivo:** Consolidar o pedido com transparência total de valores e pagamento rápido.
* **Elementos:**
  * Lista dos itens adicionados com opção rápida de editar quantidade ou remover.
  * Seletor de modalidade: **Entrega (Delivery)** ou **Retirada no Balcão**.
  * Card de endereço confirmado com tempo estimado (`30 - 40 min`).
  * Seleção de forma de pagamento (*Pix Instantâneo*, *Cartão na Entrega*, *Vale-Refeição*).
  * Resumo financeiro claro (Subtotal, Taxa de Entrega e Total) + botão *"Finalizar Pedido"*.

### Tela 05: Acompanhamento do Pedido (Status em Tempo Real)
* **Objetivo:** Reduzir a ansiedade pós-compra com feedback visual claro das etapas.
* **Elementos:**
  * Número do pedido (`#4082`) e previsão exata de chegada.
  * Linha do tempo visual (Stepper vertical) com 4 estágios:
    1. *Pedido Confirmado* (Concluído)
    2. *Em Preparo na Cozinha* (Ativo)
    3. *Saiu para Entrega* (Pendente)
    4. *Entregue* (Pendente)
  * Botão de suporte rápido caso precise falar com o restaurante.

---

## 2. Lógica de Navegação (Figma Prototype)

* **Transições:** Uso de `Smart Animate` (300ms, *Ease Out*) para abertura de modais, troca de filtros de categoria e atualização do contador de quantidade.
* **Navegação Principal:** Fluxo linear entre *Home* $\rightarrow$ *Detalhes do Prato* $\rightarrow$ *Sacola* $\rightarrow$ *Status do Pedido*, com retorno acessível em todas as etapas via ícone de voltar no cabeçalho.
* **Scroll:** Rolagem vertical fluida na *Home* mantendo o cabeçalho e a barra inferior (`bottom-nav`) fixos (`Fix position when scrolling`).