# 📊 Diário de Glicose

Aplicativo web (HTML puro) para monitoramento pessoal de glicemia, otimizado para uso no celular.

## ✨ Funcionalidades

- **Registro de medições** — data/hora (fuso horário local), valor em mg/dL, período e observação
- **Estatísticas automáticas** — média, máxima, mínima e % na faixa ideal (70–140 mg/dL)
- **Gráfico de linha** — evolução das medições ao longo do tempo (Chart.js)
- **Histórico em tabela** — ordenado do mais recente, com exclusão individual
- **Exportar CSV** — para análise em planilhas
- **Exportar PDF** — via impressão do navegador
- **Envio por WhatsApp** — envia cada medição formatada diretamente para a médica
- **Dados locais** — tudo salvo no `localStorage` do navegador (sem servidor, sem internet obrigatória)

## 🚀 Como usar

1. Abra o arquivo `teste.html` diretamente no navegador (celular ou computador)
2. Na caixa verde, cadastre o número de WhatsApp da sua médica (formato: `55` + DDD + número, ex: `5511999998888`)
3. Registre suas medições de glicose normalmente
4. Após cada medição, clique no botão verde para enviar via WhatsApp

## 📁 Estrutura

```
glicose/
└── teste.html   # Aplicativo completo em arquivo único
└── README.md    # Esta documentação
```

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML5 / CSS3 / JavaScript | Interface e lógica |
| [Chart.js](https://www.chartjs.org/) | Gráfico de glicose |
| localStorage | Persistência dos dados |
| WhatsApp API (`wa.me`) | Envio de medições |

## ⚠️ Observações

- Os dados ficam **apenas no navegador**. Não apague os dados do navegador ou troque de dispositivo sem exportar o CSV antes.
- O horário registrado usa sempre o **fuso horário local** do dispositivo.
- Valores de referência usados: Normal = 70–140 mg/dL | Alto = 141–180 mg/dL | Muito Alto = >180 mg/dL
