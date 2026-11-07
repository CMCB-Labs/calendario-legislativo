# 📅 Calendário Legislativo - CMCB

Calendário interativo oficial das **Sessões Ordinárias, Sessões Extraordinárias, Reuniões das Comissões Permanentes e Feriados** da Câmara Municipal de Coronel Barros/RS para o ano legislativo de 2026.

---

## 🌐 Acesso Direto
- **URL Oficial:** [https://cmcb-labs.github.io/calendario-legislativo/](https://cmcb-labs.github.io/calendario-legislativo/)

---

## ⚖️ Regras Regimentais Aplicadas
- **Sessões Ordinárias:** Quinzenais, nas segundas-feiras, às 18h.
- **Reuniões de Comissões Permanentes:** Quinzenais, nas segundas-feiras, às 17h35.
- **Transferência por Feriado (Art. 10, § 3º da Lei Orgânica Municipal):** Em caso de feriado ou ponto facultativo na segunda-feira, a sessão ou reunião é automaticamente transferida para a terça-feira subsequente.
- **Feriados Oficiais 2026:** Feriados nacionais, estaduais do RS e municipais de Coronel Barros incluídos no calendário.

---

## 💻 Código para Incorporação (Embed / Iframe no Portal)

### 1. Para Páginas ou Janela (Window) do Plone (Recomendado)
```html
<iframe 
  src="https://cmcb-labs.github.io/calendario-legislativo/?embed=1" 
  width="100%" 
  height="780" 
  frameborder="0" 
  scrolling="no" 
  style="border: none; width: 100%; min-height: 600px; overflow: hidden; display: block;">
</iframe>
```

### 2. Para Notícias ou Matérias (Sem cabeçalho superior)
```html
<iframe 
  src="https://cmcb-labs.github.io/calendario-legislativo/?embed=1&hide_header=1" 
  width="100%" 
  height="720" 
  frameborder="0" 
  scrolling="no" 
  style="border: none; width: 100%; min-height: 550px; overflow: hidden; display: block;">
</iframe>
```

> **Parâmetros da URL:**
> - `?embed=1`: ativa modo embutido com fundo transparente e remoção de margens extras.
> - `&hide_header=1`: oculta o cabeçalho superior verde institucional.
> - **Zero Scrollbar:** O painel dispara automaticamente eventos `sapl-resize` via `postMessage`, redimensionando a altura do iframe de acordo com o tema da Câmara.
