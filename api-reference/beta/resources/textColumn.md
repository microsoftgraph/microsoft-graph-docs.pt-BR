---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 87a5e27544a49613d1d1e44cd6f3e0e3b7fcf8c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822565"
---
# <a name="textcolumn-resource-type"></a>Tipo de recurso TextColumn

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
