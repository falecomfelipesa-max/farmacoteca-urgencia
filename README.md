# 💊 Farmacoteca de Urgência e Emergência

> Aplicação web standalone para consulta rápida de medicamentos em cenários de urgência e emergência pré-hospitalar e intra-hospitalar. Inclui **calculadora de doses por peso** para uso à beira do leito.

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Offline](https://img.shields.io/badge/offline-100%25-green.svg)]()

---

## 🎯 O que é

Ferramenta de consulta médica para **profissionais da saúde** atuando em urgência/emergência. Único arquivo HTML, sem dependências externas, funciona offline em qualquer dispositivo com navegador (celular, tablet, desktop). Pode ser hospedado em qualquer lugar (GitHub Pages, intranet hospitalar, pendrive, Google Drive).

Cobre os **32 medicamentos essenciais** do carrinho de emergência e maleta SAMU brasileiro, com posologia para adulto, pediátrico e gestante, indicações, mecanismo, preparo, precauções e reações adversas.

## ✨ Funcionalidades

- 🔍 **Busca instantânea** — por nome, sinônimo, classe terapêutica, indicação ou tag
- ⚡ **Calculadora de doses por peso** — informe o peso uma vez (persistido em `localStorage`) e veja todas as doses calculadas automaticamente para cada medicamento
- 🏷️ **22 filtros por cenário clínico** — PCR, Arritmias, Choque/DVA, Anafilaxia, Broncoespasmo, EAP/IC, SCA, Convulsão, CAD, Sedação/IOT, etc.
- 📱 **Responsivo** — funciona bem em celular à beira do leito e em desktop
- 🌑 **Dark theme** otimizado para uso noturno em plantão
- 🖨️ **Imprimível** — CSS @media print configurado
- 🆘 **Atalhos** — tecla `/` foca a busca, `Esc` fecha modais
- 💾 **100% offline** — abre direto do disco, sem servidor

## 🧪 Medicamentos cobertos

Adrenalina/Epinefrina, Água destilada, Aminofilina, Amiodarona, Atropina, Brometo de Ipratrópio, Cloreto de potássio, Cloreto de sódio, Deslanosídeo, Dexametasona, Diazepam, Diclofenaco, Dipirona, Dobutamina, Dopamina, Escopolamina (hioscina), Fenitoína/Hidantoína, Fenobarbital, Furosemida, Glicose, Haloperidol, Hidrocortisona, Insulina, Isossorbida, Lidocaína, Meperidina, Midazolam, Ringer Lactato, Soro Glico-Fisiológico, Soro Glicosado.

## 🧮 Calculadora de doses

Para os medicamentos críticos, a calculadora gera automaticamente:

- **Adrenalina** — bolus em PCR pediátrica, anafilaxia IM por kg, crupe NBZ, BIC em mL/h
- **Amiodarona** — bolus em PCR pediátrica
- **Atropina** — bradicardia pediátrica, organofosforado, pré-IOT
- **Dobutamina / Dopamina / Adrenalina BIC** — tabela completa de mcg/kg/min → mL/h
- **Diazepam / Midazolam / Fenitoína / Fenobarbital** — doses para crise convulsiva
- **Insulina** — BIC em CAD (UI/h e mL/h)
- **Furosemida** — dose em EAP por kg
- **Glicose** — bolus de SG 25%, 10% e 50% conforme idade
- **Lidocaína** — dose em PCR e dose máxima segura para anestesia local
- **Ringer Lactato** — Fórmula de Parkland para queimadura (tabela por %SCQ)
- **Soro Glicosado** — VIG (Velocidade de Infusão de Glicose) pediátrica
- **KCl, Brometo de Ipratrópio, Dexametasona, Hidrocortisona, Aminofilina, Meperidina, Dipirona, e mais**

## 🚀 Como usar

### Online (GitHub Pages)

```
https://<seu-usuario>.github.io/farmacoteca-urgencia/
```

### Local

Basta abrir o arquivo `index.html` em qualquer navegador moderno:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

### Servir localmente (opcional)

```bash
# Python 3
python3 -m http.server 8000

# Node.js
npx serve .
```

## 📚 Fontes consultadas

As doses e condutas derivam de protocolos brasileiros consolidados e diretrizes internacionais:

- **AHA ACLS / PALS 2020** (parada cardiorrespiratória)
- **Sociedade Brasileira de Cardiologia** — Diretrizes de IAM, IC, EAP, Arritmias
- **Sociedade Brasileira de Pediatria** — Anafilaxia, Crupe, Crise Convulsiva
- **Sociedade Brasileira de Diabetes** — CAD 2025
- **Protocolos SAMU 192** (RS, DF, SP, Sorocaba, Fortaleza)
- **GINA 2023** (asma)
- **Surviving Sepsis Campaign 2021**
- **ATLS 10ª edição** (trauma)
- **Pathways Hospital Israelita Albert Einstein**
- **AES Guidelines** (status epilepticus)
- **Bulas ANVISA** dos fármacos individuais

Cada medicamento lista suas fontes específicas no card.

## ⚠️ Aviso médico

Esta ferramenta é um **apoio de consulta rápida** para profissionais médicos. As posologias resumidas requerem sempre:

- Verificação no contexto clínico individual
- Confirmação na bula atualizada do produto utilizado
- Ponderação de fatores do paciente (peso real, função renal/hepática, alergias, interações)
- **Não substitui julgamento clínico**

A calculadora foi cuidadosamente codificada com limites superiores e inferiores onde aplicável (ex.: adrenalina IM ped máx 0,3 mg), mas o profissional **sempre deve conferir o cálculo manualmente** antes da administração.

## 🛠️ Stack técnica

- HTML5 / CSS3 / JavaScript vanilla
- Sem build, sem dependências, sem CDN
- `localStorage` para persistir peso do paciente entre sessões
- Tamanho final: ~120 KB (sem minificar)

## 🤝 Contribuindo

Sugestões de correção de doses, novos medicamentos ou melhorias de usabilidade são bem-vindas via Issue ou Pull Request.

## 📄 Licença

[MIT](LICENSE) — uso livre para fins clínicos, educacionais e comerciais.

## ✍️ Autor

Desenvolvido por **Felipe** ([Aulus Araújo Neto](https://github.com/)) — médico, desenvolvedor full-stack e fundador da [AulusTech](https://aulustech.com.br).

Compilado com apoio de IA (Claude/Anthropic) e revisão clínica.

---

**Versão:** 1.0.0 · **Última atualização:** 2026-05
