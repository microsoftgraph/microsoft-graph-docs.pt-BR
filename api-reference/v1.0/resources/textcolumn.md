---
author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 62711f2f44004e5b3d594eb472b7c018205d9e31
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239271"
---
# <a name="textcolumn-resource-type"></a>Tipo de recurso TextColumn

Namespace: microsoft.graph

**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.

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
| **allowMultipleLines**          | booliano | Se deseja permitir várias linhas de texto.
| **appendChangesToExistingText** | booliano | Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.
| **linesForEditing**             | int32   | O tamanho da caixa de texto.
| **maxLength**                   | int32   | O número máximo de caracteres para o valor.
| **textType**                    | string  | O tipo de texto sendo armazenado. Deve ser `plain` ou `richText`

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

