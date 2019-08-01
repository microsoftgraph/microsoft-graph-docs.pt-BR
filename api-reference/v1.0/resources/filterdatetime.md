---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e2938c151e052372df1b959e6e24d4a2c0d94ea4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032456"
---
# <a name="filterdatetime-resource-type"></a>Tipo de recurso FilterDatetime

Indica como filtrar uma data ao filtrar valores.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|data|string|A data no formato ISO8601 usada para filtrar os dados.|
|especificidade|cadeia de caracteres|Como a data específica deve ser usada para manter os dados. Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009. Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
