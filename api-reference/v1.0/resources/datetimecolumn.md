---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: ba650ccbe307ba286cf2182bda35a21f3c675114
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480170"
---
# <a name="datetimecolumn-resource-type"></a>Tipo de recurso DateTimeColumn

**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **dateTimeColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade      | Tipo               | Descrição
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | string             | Como o valor deve ser apresentado na experiência do usuário. Deve ser `default`, `friendly` ou `standard`. Consulte abaixo para ver mais detalhes. Se não for especificado, é tratado como `default`.
| **format**         | string             | Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora. Deve ser `dateOnly` ou `dateTime`

## <a name="displayas-options"></a>Opções de displayas

| Valor        | Descrição
|:-------------|:--------------------------------------------------------------
| **default**  | Usa o processamento de renderização padrão na UX.
| **amigável** | Usa uma representação amigável relativa (ex. "hoje às 15:00")
| **standard** | Usa a representação padrão absoluta (ex. "10/05/2017 15:20")


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
