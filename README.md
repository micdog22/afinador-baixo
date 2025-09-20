# Afinador de Baixo — Afinador Online (HTML + CSS + JS)

Afinador simples feito em uma única página (`index.html`) usando a **Web Audio API**. Funciona no navegador (desktop e mobile) e pode ser publicado facilmente no **GitHub Pages**.

## Como funciona
- **Microfone:** ao clicar em “Usar microfone”, a página captura o áudio e executa **detecção de frequência** por **autocorrelação**. A nota mais próxima e o desvio em **cents** são exibidos junto de um indicador visual.
- **Nota de referência:** o botão “Tocar nota” gera um tom senoidal usando um **OscillatorNode** para a corda selecionada.
- **Calibração:** ajuste da referência **A4** (padrão 440 Hz) no controle deslizante.
- **Cordas disponíveis**
- E1: 41.2 Hz
- A1: 55.0 Hz
- D2: 73.42 Hz
- G2: 98.0 Hz

## Como publicar no GitHub Pages
1. Crie um repositório e envie os arquivos desta pasta (afinador-baixo).
2. Em **Settings → Pages**, selecione a branch (por exemplo `main`) e a pasta **/root**.
3. Acesse a URL pública gerada (ex.: `https://seu-usuario.github.io/afinador-baixo/`).

## Dicas de uso
- Use em ambiente silencioso e toque corda **solta**.
- Em dispositivos móveis, o navegador só libera microfone em **HTTPS** (GitHub Pages já usa HTTPS).
- Se o ponteiro oscila muito, amorteça a corda e toque novamente.

## Licença
MIT.
