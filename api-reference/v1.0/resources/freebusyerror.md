---
title: tipo de recurso freeBusyError
description: Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8e069aef1d26a409e9ebe29a516136a952604ee6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531381"
---
# <a name="freebusyerror-resource-type"></a>tipo de recurso freeBusyError

Namespace: microsoft.graph

Representa informações de erro da tentativa de obter a disponibilidade de um usuário, lista de distribuição ou recurso.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|mensagem |String |Descreve o erro. |
|responseCode |String |O código de resposta da consulta para a disponibilidade do usuário, lista de distribuição ou recurso. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
