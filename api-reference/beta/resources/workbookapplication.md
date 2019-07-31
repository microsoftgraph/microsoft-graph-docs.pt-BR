---
title: tipo de recurso workbookApplication
description: Representa o workbookApplication do Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 71c7c92e623fc2a9c05b9e1e8448f329615c51e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964106"
---
# <a name="workbookapplication-resource-type"></a>tipo de recurso workbookApplication

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o aplicativo Excel que gerencia a pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookApplication](../api/workbookapplication-get.md) | [workbookApplication](workbookapplication.md) |Leia as propriedades e os relacionamentos do objeto workbookApplication.|
|[Calculate](../api/workbookapplication-calculate.md)|Nenhum|Recalcula todas as pastas de trabalho abertas no Excel no momento.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|cálculomode|string|Retorna o modo de cálculo usado na pasta de trabalho. Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
