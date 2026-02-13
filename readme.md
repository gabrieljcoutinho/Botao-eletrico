# Voltage Animated Button

Este projeto apresenta um botão de alta fidelidade visual que utiliza **SVG Filters** e **CSS Animations** para criar um efeito de eletricidade e partículas magnéticas ao interagir com o elemento.

## Funcionalidades e Efeitos

* **Efeito de Voltagem:** O uso de filtros SVG (`feTurbulence` e `feDisplacementMap`) cria uma distorção orgânica nas linhas ao redor do botão, simulando descargas elétricas reais.
* **Glow Dinâmico:** Aplicação de `feGaussianBlur` para criar um brilho neon que acompanha o movimento dos raios.
* **Sistema de Partículas:** Pequenas esferas (dots) são disparadas em direções opostas através de animações de translação e escala, reforçando a ideia de liberação de energia.
* **Interatividade Hover:** O estado de animação é ativado apenas quando o usuário passa o mouse sobre o botão, otimizando o processamento visual.

## Detalhes Técnicos

### SVG e Filtros
A parte mais complexa do projeto está no filtro de identificação `#glow`. Ele combina ruído fractal com mapas de deslocamento para garantir que as linhas de "raio" nunca pareçam estáticas ou perfeitamente retas.

### Animações CSS
* **spark-1 & spark-2:** Controlam o `stroke-dashoffset` dos paths de SVG para criar o movimento de fluxo elétrico.
* **fly-up & fly-down:** Gerenciam a trajetória das partículas, utilizando variações de `opacity` e `transform: translateY` para simular dissipação.

## Estrutura do Projeto

* `index.html`: Contém a estrutura do botão, os paths do SVG e a definição dos filtros de renderização.
* `style.css`: Gerencia o posicionamento absoluto dos elementos, o design do botão e toda a lógica de animação por keyframes.

## Tecnologias

* HTML5
* CSS3 (Animations & Transforms)
* SVG (Filters & Path Animation)
