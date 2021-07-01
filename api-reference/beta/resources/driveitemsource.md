---
author: MarcMroz
description: O driveItemSource contém metadados sobre o aplicativo de origem em que o item de unidade foi criado.
title: Tipo de recurso driveItemSource
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: a403f570ac550b62f9c0e7fa0c3c2fa9758e1772
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236287"
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
