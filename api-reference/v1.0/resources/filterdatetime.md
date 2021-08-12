---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d31c8718f96f1e89f2e6fbb31413ee9c19d08b0e97758d384a1d568d2edeb657
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216921"
---
# <a name="filterdatetime-resource-type"></a>Tipo de recurso FilterDatetime

Namespace: microsoft.graph

Indica como filtrar uma data ao filtrar valores.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|data|cadeia de caracteres|A data no formato ISO8601 usada para filtrar os dados.|
|especificidade|string|Como a data específica deve ser usada para manter os dados. Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009. Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.|

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

