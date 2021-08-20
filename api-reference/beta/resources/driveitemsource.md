---
author: MarcMroz
description: O driveItemSource contém metadados sobre o aplicativo de origem em que o item de unidade foi criado.
title: Tipo de recurso driveItemSource
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 98076060791424e7f84a4bee32c12a3eca1238003b413d0b0c53ce18c97a21d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206911"
---
# <a name="driveitemsource-resource-type"></a>Tipo de recurso driveItemSource

Contém metadados sobre a origem do item de unidade.

Ele está disponível na propriedade de origem dos [recursos driveItem.][item-resource]

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo                       | Descrição                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| **application**          | driveItemSourceApplication | Valor de enumeração que indica o aplicativo de origem onde o arquivo foi criado.              |
| **externalId**           | cadeia de caracteres                     | O identificador externo do item de unidade da fonte.                                      |

### <a name="driveitemsourceapplication-values"></a>valores driveItemSourceApplication

| Valor               | Descrição                                       |
|:--------------------|:--------------------------------------------------|
| teams               | O aplicativo é Teams.                         |
| yammer              | O aplicativo é Yammer.                        |
| sharePoint          | O aplicativo é SharePoint.                    |
| oneDrive            | O aplicativo é OneDrive.                      |
| stream              | O aplicativo é Stream.                        |
| powerPoint          | O aplicativo é PowerPoint                     |
| office              | O aplicativo é Office                         |
| unknownFutureValue  | Valor do marcador para compatibilidade futura.            |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "application",
    "externalId",
  ],
  "@odata.type": "microsoft.graph.driveItemSource"
}-->

```json
{
  "application": "string",
  "externalId" : "string"
}
```

## <a name="see-also"></a>Confira também

Para obter mais informações sobre as facetas em um driveItem, [consulte driveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The driveItemSource facet provides information about drive item source.",
  "keywords": "driveItemSoruce,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/driveItemSource"
} -->
