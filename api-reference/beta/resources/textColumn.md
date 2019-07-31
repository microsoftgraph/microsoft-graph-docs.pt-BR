---
author: JeremyKelley
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6681875328695d2e67cc10508f47183fcedb0df4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964337"
---
# <a name="textcolumn-resource-type"></a>Tipo de recurso TextColumn

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

| Nome da propriedade                   | Tipo   | Descrição
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | string | Se deseja permitir várias linhas de texto.
| **appendChangesToExistingText** | string | Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.
| **linesForEditing**             | int    | O tamanho da caixa de texto.
| **maxLength**                   | int    | O número máximo de caracteres para o valor.
| **textType**                    | string | O tipo de texto sendo armazenado. Deve ser `plain` ou `richText`

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
