# 01. Briefing e Análise de UX Research

## 1. Briefing do Projeto
* **Cliente:** Restaurante Sabor Brasileiro (Fictício)
* **Produto:** Aplicativo Mobile de Pedidos Próprios (*Sabor Brasileiro Express*)
* **Objetivo Principal:** Reduzir a dependência de marketplaces de terceiros (que cobram taxas de até 27% por pedido) e eliminar gargalos no atendimento manual via WhatsApp nos horários de pico (11h30 às 13h30).
* **Público-Alvo:** Trabalhadores de escritórios, estudantes universitários e moradores locais (22 a 50 anos) que buscam refeições rápidas, bem servidas, com preço justo e transparência no tempo de entrega.
* **Plataforma:** Mobile (iOS e Android) — Resolução base de projeto: `390 x 844 px` (iPhone 14/15).

---

## 2. Análise do Problema e Dores Identificadas
1. **Lentidão no atendimento via chat:** Clientes desistem de pedir quando demoram mais de 5 minutos para receber o cardápio em PDF ou confirmar o valor do frete.
2. **Falta de personalização clara:** Dificuldade para solicitar trocas simples de acompanhamento (ex: trocar fritas por salada) sem gerar erros na cozinha.
3. **Insegurança na entrega:** Falta de visibilidade sobre o status real do preparo e saída do motoboy.

---

## 3. Matriz CSD (Certezas, Suposições e Dúvidas)

| Certezas | Suposições | Dúvidas |
| :--- | :--- | :--- |
| O pico de pedidos ocorre entre 11h30 e 13h30. | Clientes preferem pagar via Pix se houver confirmação automática. | Qual o valor mínimo ideal para oferecer frete grátis? |
| As taxas dos apps terceiros reduzem a margem de lucro. | Um programa de pontos simples aumenta a recorrência semanal. | Os clientes preferem agendar pedidos ou pedir na hora? |
| O cardápio atual em PDF confunde o cliente no celular. | Fotos reais dos pratos aumentam a conversão de sobremesas. | Quantos passos são toleráveis antes do checkout? |

---

## 4. Proto-Persona

* **Nome:** Mariana Costa, 32 anos
* **Profissão:** Analista Administrativa
* **Contexto:** Trabalha em modelo híbrido e tem apenas 1 hora de almoço. Costuma pedir marmitas executivas 3 vezes por semana.
* **Dores:** Odeia ter que mandar "Oi, tudo bem?" no WhatsApp e esperar resposta para saber o prato do dia. Fica frustrada quando o pedido atrasa sem aviso.
* **Objetivos:** Abrir o app, repetir seu último pedido ou escolher o prato do dia em menos de 2 minutos, pagar no Pix e acompanhar a chegada.

---

## 5. User Flow (Fluxo Principal de Pedido)

```text
[Splash Screen] 
      │
      ▼
[Home / Cardápio] ──► (Busca ou Filtro por Categoria)
      │
      ▼
[Detalhes do Prato] ──► (Escolhe Acompanhamento + Observações)
      │
      ▼
[Adicionar ao Carrinho] ──► (Continua comprando ou vai para Sacola)
      │
      ▼
[Checkout / Sacola] ──► (Confirma Endereço + Seleciona Pix/Cartão)
      │
      ▼
[Acompanhamento do Pedido] ──► (Recebido -> Em Preparo -> Saiu para Entrega)