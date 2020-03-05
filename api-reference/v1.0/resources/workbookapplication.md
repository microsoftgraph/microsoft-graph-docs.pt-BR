---
title: tipo de recurso workbookApplication
description: Representa o aplicativo Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d4b2833910d22696ee95ed707469f6da2068453c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446720"
---
# <a name="workbookapplication-resource-type"></a>tipo de recurso workbookApplication

Namespace: Microsoft. Graph

Representa o aplicativo Excel que gerencia a pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookApplication](../api/workbookapplication-get.md) | [workbookApplication](workbookapplication.md) |Leia as propriedades e os relacionamentos do objeto workbookApplication.|
|[Calculate](../api/workbookapplication-calculate.md)|Nenhum|Recalcula todas as pastas de trabalho abertas no Excel no momento.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|cálculomode|string|Retorna o modo de cálculo usado na pasta de trabalho. Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
