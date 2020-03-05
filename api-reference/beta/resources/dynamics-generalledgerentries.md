---
title: tipo de recurso generalLedgerEntries
description: Uma entrada de contabilidade no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f1dc4ec7bb3fa30f7dc6362c850893953c4aa6aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503975"
---
# <a name="generalledgerentries-resource-type"></a>tipo de recurso generalLedgerEntries

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|lastModifiedDateTime|datetime               |A última data/hora em que a entrada G/L foi modificada.|


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

