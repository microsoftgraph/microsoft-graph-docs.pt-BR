---
title: tipo de recurso de foto
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.date: 09/10/2017
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: bc253cd90a75438f627cf00c55551cfb8bc12d01
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176355"
---
# <a name="photo-resource-type"></a>tipo de recurso de foto

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).

> [!NOTE]
> Atualmente, somente **takenDateTime** está disponível OneDrive for Business e SharePoint.

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo          | Descrição                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|cameraMake         |String         | Fabricante da câmera. Somente leitura.                                            |
|cameraModel        |String         | Modelo da câmera. Somente leitura.                                                   |
|exposureDenominator|Duplo         | O denominador da fração do tempo de exposição da câmera. Somente leitura. |
|exposureNumerator  |Duplo         | O numerador da fração do tempo de exposição da câmera. Somente leitura.   |
|fNumber            |Double         | O valor de f-stop da câmera. Somente leitura.                               |
|focalLength        |Double         | A distância focal da câmera. Somente leitura.                               |
|iso                |Int32          | O valor de ISO da câmera. Somente leitura.                                  |
|orientation        |Int16          | O valor de orientação da câmera. Gravável no OneDrive Personal.      |
|takenDateTime      |DateTimeOffset | A data e a hora em que a foto foi tirada no horário UTC. Somente leitura.              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.photo",
  "baseType": null
}-->

```json
{
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The photo resource provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": ""
}-->


