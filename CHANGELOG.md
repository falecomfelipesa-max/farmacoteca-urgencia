# Changelog

Todas as mudanças relevantes deste projeto são documentadas aqui.
O formato segue [Keep a Changelog](https://keepachangelog.com/pt-BR/).

## [2.0.0] — 2026-05-31
### Adicionado
- **52 novos medicamentos** da norma 2.6 (lista oficial de medicamentos da unidade de urgência), totalizando **84 medicamentos**.
  - Antibióticos: ampicilina, penicilina G cristalina, oxacilina, cefalotina, cefalexina, cloranfenicol, gentamicina, sulfametoxazol+trimetoprim.
  - Cardiovascular/HAS: captopril, enalapril/enalaprilato, hidralazina, clonidina, metildopa, nifedipina, nitroprussiato de sódio, metoprolol, propranolol, verapamil, digoxina.
  - Obstétrico: sulfato de magnésio, metilergometrina, (nifedipina/hidralazina como uterotônico/anti-HAS gestacional).
  - Antídotos/intoxicação: carvão ativado, flumazenil, gluconato de cálcio, bicarbonato de sódio, tiamina, vitamina K, biperideno.
  - Neuro/psiquiatria: carbamazepina, amitriptilina, clordiazepóxido, clorpromazina.
  - Respiratório: salbutamol, fenoterol, metilprednisolona.
  - Analgesia/sintomáticos: paracetamol, cetoprofeno, tramadol, codeína, metoclopramida, prometazina, omeprazol, ranitidina, complexo B.
  - Outros: manitol, sais de reidratação oral, nistatina, sulfadiazina de prata, tobramicina colírio, óleo mineral, clister glicerinado, bupivacaína.
- **Tema claro (light mode)** com alternância via botão no cabeçalho e atalho de teclado **T**; preferência persistida e detecção automática do tema do sistema.
- Novos filtros de cenário: **Antibióticos**, **Obstétrico**, **Gastro/Náusea** e **Outros**.
- Calculadoras de dose por peso para os novos medicamentos (paracetamol, salbutamol, fenoterol, sulfato de magnésio, gluconato de cálcio, bicarbonato, manitol, carvão ativado, flumazenil, tramadol, metoclopramida, prometazina, biperideno, hidralazina, verapamil, propranolol, gentamicina e antibióticos por mg|UI/kg/dia, entre outros).

### Notas
- "Glicose isotônica/hipertônica" e "Soro Fisiológico" da lista oficial estão cobertos como sinônimos dos cards já existentes (sem duplicação).
- Doses validadas em fontes brasileiras/internacionais (MS, FEBRASGO, SBC, SBP, GINA, AHA ACLS/Intoxicações, Einstein Pathways, CCIH, bulas ANVISA).

## [1.0.0] — 2026-05-31
### Adicionado
- Versão inicial: 32 medicamentos do carrinho de emergência, busca instantânea, filtros por cenário, calculadora de dose por peso e tema escuro.
