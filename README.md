# Dra. Tábada Microni | Biomédica Esteta

Site de apresentação e agendamento (Contagem, MG). Página única, sem dependências: abra `index.html`.

## Como o agendamento funciona aqui

O visitante escolhe tratamento, dia e horário e envia uma mensagem pronta pelo WhatsApp da clínica.

Esta cópia é estática. O painel da clínica (agenda, horários, cancelamentos, publicação) só funciona na versão hospedada no claude.ai, que oferece banco de dados. Aqui os horários são ilustrativos, a menos que exista um arquivo `agenda.json` ao lado do `index.html`, no formato:

```json
{ "v": 1, "generatedAt": "2026-11-02T12:00:00Z", "minNotice": 12,
  "days": { "2026-11-05": ["09:00", "10:00"], "2026-11-06": [] } }
```

Dias ausentes ficam fechados e dias com lista vazia aparecem como "lotado".

## Antes de divulgar

- As condições do mês são exemplos.
- Falta o número do CRBM no rodapé.
