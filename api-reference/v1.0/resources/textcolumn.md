---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: b5c41091b9193aabc36ee04e9dcc310bfc110af1
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264284"
---
# <a name="textcolumn-resource-type"></a>Tipo de recurso TextColumn

**textColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são texto.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **textColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade                   | Tipo    | Descrição
|:--------------------------------|:--------|:---------------------------------
| **allowMultipleLines**          | booleano | Se deseja permitir várias linhas de texto.
| **appendChangesToExistingText** | booleano | Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.
| **linesForEditing**             | int32   | O tamanho da caixa de texto.
| **maxLength**                   | int32   | O número máximo de caracteres para o valor.
| **textType**                    | sequência de caracteres  | O tipo de texto sendo armazenado. Deve ser `plain` ou `richText`

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->
