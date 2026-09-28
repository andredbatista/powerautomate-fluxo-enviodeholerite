# Automação de Envio e Confirmação de Recebimento de Holerites

## Visão Geral

Esta solução automatiza todo o processo de distribuição e confirmação de recebimento de holerites utilizando Microsoft SharePoint, Power Automate e Microsoft Approvals.

O objetivo é eliminar atividades manuais de impressão, entrega física e controle de recebimento dos holerites, proporcionando rastreabilidade, auditoria e armazenamento centralizado dos documentos.

---

## Funcionalidades

### 1. Distribuição Automática de Holerites

O fluxo monitora uma biblioteca de documentos no SharePoint onde os holerites em PDF são armazenados.

Quando um arquivo é marcado para envio:

- Identifica automaticamente o colaborador através da matrícula presente no nome do arquivo.
- Consulta a lista de colaboradores no SharePoint.
- Obtém o e-mail do colaborador correspondente.
- Envia o holerite em PDF por e-mail.
- Registra as informações de envio.
- Atualiza o status do documento para "Enviado".
- Armazena a data e hora do envio.

### Exemplo de nomenclatura de arquivo

```text
1001_holerite_2026-09.pdf
