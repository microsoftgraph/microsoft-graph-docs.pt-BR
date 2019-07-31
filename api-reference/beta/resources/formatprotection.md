---
title: Tipo de recurso FormatProtection
description: Representa a proteção de formatação de um objeto range.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 036c09c1d5e4dfec043e6a1dc612aa728d6588f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973538"
---
# <a name="formatprotection-resource-type"></a>Tipo de recurso FormatProtection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a proteção de formatação de um objeto range.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get FormatProtection](../api/formatprotection-get.md) | [FormatProtection](formatprotection.md) |Leia as propriedades e os relacionamentos do objeto formatProtection.|
|[Update](../api/formatprotection-update.md) | [FormatProtection](formatprotection.md)  |Atualize o objeto FormatProtection. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formulaHidden|booliano|Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.|
|locked|booliano|Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
