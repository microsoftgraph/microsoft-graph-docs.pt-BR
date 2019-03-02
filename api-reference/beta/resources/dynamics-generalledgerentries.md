---
title: tipo de recurso generalLedgerEntries
description: Uma entrada de contabilidade no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365756"
---
# <a name="generalledgerentries-resource-type"></a>tipo de recurso generalLedgerEntries
Representa um objeto generalLedgerEntry no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:-------------|:-------------|:----------|
|[Obter generalLedgerEntries](../api/dynamics-generalledgerentries-get.md)|generalLedgerEntries|Obter um objeto de entrada G/L.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                  |Descrição                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|id                  |numéricos                |A identificação exclusiva da entrada G/L.              |
|postingDate         |data                   |Especifica a data de lançamento da entrada G/L. |
|documentNumber      |Cadeia de caracteres, tamanho máximo 20|Especifica o número do documento da entrada G/L.|
|documentType        |string                 |Especifica o tipo de documento da entrada G/L.|
|accountId           |GUID                   |Especifica a AccountId da entrada G/L.    |
|accountNumber       |Cadeia de caracteres, tamanho máximo 20|Especifica o accountNumber da entrada G/L.|
|description         |Cadeia de caracteres, tamanho máximo 50|Especifica a descrição da entrada G/L.  |
|debitAmount         |numéricos                |Especifica o debitAmount da entrada G/L.  |
|creditAmount        |numéricos                |Especifica o creditAmount da entrada G/L. |
|lastModifiedDateTime|DateTime               |A última data/hora em que a entrada G/L foi modificada.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

