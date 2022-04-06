---
author: JeremyKelley
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.date: 09/11/2017
title: TextColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8a6e8d3a06c3d34a321ec2fb5ff5d83586accb56
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724284"
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
