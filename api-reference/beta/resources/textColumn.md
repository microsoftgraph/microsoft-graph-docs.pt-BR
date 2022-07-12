---
author: JeremyKelley
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.date: 09/11/2017
title: TextColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: workbooks-and-charts
ms.openlocfilehash: a26653663d3327bf7c434de49c2febec539f69db
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735576"
---
# <a name="textcolumn-resource-type"></a>Tipo de recurso TextColumn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Propriedade                        | Tipo   | Descrição                                                                   |
| :------------------------------ | :----- | :---------------------------------------------------------------------------- |
| **allowMultipleLines**          | string | Se deseja permitir várias linhas de texto.                                      |
| **appendChangesToExistingText** | string | Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele. |
| **linesForEditing**             | int    | O tamanho da caixa de texto.                                                     |
| **maxLength**                   | int    | O número máximo de caracteres para o valor.                               |
| **textType**                    | string | O tipo de texto sendo armazenado. Deve ser `plain` ou `richText`           |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->
