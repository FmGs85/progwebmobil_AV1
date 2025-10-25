# 🍅 Fokus - Aplicativo Pomodoro

Aplicativo de gerenciamento de tempo baseado na técnica Pomodoro, desenvolvido em React Native como parte da Avaliação 1 da disciplina de Programação Mobile 1.

## 📋 Sobre o Projeto

O **Fokus** é um timer Pomodoro que ajuda a melhorar a produtividade através de ciclos de trabalho focado e pausas planejadas. O aplicativo permite alternar entre três modos:

- **Foco**: 25 minutos de trabalho concentrado
- **Pausa Curta**: 5 minutos de descanso
- **Pausa Longa**: 15 minutos de descanso prolongado

## 🚀 Tecnologias Utilizadas

- **React Native**: Framework para desenvolvimento mobile
- **Expo**: Plataforma para desenvolvimento e build
- **React Hooks**: `useState`, `useRef` para gerenciamento de estado
- **React Native SVG**: Para renderização dos ícones personalizados

## ✨ Funcionalidades

- ⏱️ Timer countdown com três modos diferentes (Foco, Pausa Curta, Pausa Longa)
- ▶️ Botão de play/pause para controlar o timer
- 🎨 Interface visual com imagens diferentes para cada modo
- 🔄 Troca dinâmica entre os modos com reset automático do timer
- 📱 Design responsivo e interface intuitiva
- 🎯 Visual minimalista com esquema de cores focado em produtividade

## 🏗️ Estrutura do Projeto

```
fokus/
├── app/
│   ├── index.jsx              # Tela principal com lógica do timer
│   ├── pomodoro.png           # Imagem do modo Foco
│   ├── short.png              # Imagem da Pausa Curta
│   └── long.png               # Imagem da Pausa Longa
└── components/
    ├── ActionButton.jsx       # Botões de seleção de modo
    ├── FokusButton.jsx        # Botão principal (Play/Pause)
    ├── Timer.jsx              # Componente de exibição do tempo
    └── Icons.jsx              # Ícones SVG (Play e Pause)
```

## 🎨 Componentes Principais

### ActionButton
Botões para alternar entre os modos (Foco, Pausa Curta, Pausa Longa). Possui estado visual ativo quando selecionado.

### FokusButton
Botão principal que controla o início e pausa do timer, com ícone dinâmico que muda entre play e pause.

### Timer
Componente responsável por exibir o tempo restante no formato MM:SS, utilizando formatação de data brasileira.

### Icons
Ícones SVG customizados para os botões de play e pause, garantindo qualidade em qualquer resolução.

## 🔧 Como Executar o Projeto

1. Clone o repositório:
```bash
git clone https://github.com/FmGs85/progwebmobil_AV1.git
cd progwebmobil_AV1
```

2. Instale as dependências:
```bash
npm install
# ou
yarn install
```

3. Execute o projeto:
```bash
npx expo start
```

4. Escaneie o QR Code com o aplicativo Expo Go no seu smartphone ou execute em um emulador.

## 💡 Lógica de Funcionamento

O aplicativo utiliza `setInterval` para decrementar os segundos a cada 1000ms (1 segundo). O estado do timer é gerenciado através de:

- **timerType**: Armazena o modo atual (foco, pausa curta ou longa)
- **seconds**: Contador de segundos restantes
- **timerRunning**: Indica se o timer está em execução
- **timerRef**: Referência ao intervalo para controle preciso

Quando o timer chega a zero, ele é automaticamente resetado para o valor inicial do modo atual.

## 🎓 Contexto Acadêmico

Este projeto foi desenvolvido como Avaliação 1 (AV1) da disciplina de **Programação Mobile 1**, demonstrando conhecimentos em:

- Desenvolvimento de aplicativos mobile com React Native
- Gerenciamento de estado com Hooks
- Componentização e reutilização de código
- Manipulação de timers e intervalos
- Estilização e design de interfaces mobile

## 📄 Licença

Projeto fictício e sem fins comerciais, desenvolvido para fins educacionais.

## 👨‍💻 Autor

Desenvolvido por **Fábio Melo Gumarães da Silva** - Aluno de Programação Mobile 1

---

⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório!
