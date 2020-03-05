---
title: tipo de recurso Photo
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bdb587e7440fd98c48f71a2611e2a34e039367dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521880"
---
# <a name="photo-resource-type"></a>tipo de recurso Photo

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).

> [!NOTE]
> Atualmente, apenas o **takenDateTime** está disponível no onedrive for Business e no SharePoint.

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo          | Descrição                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|cameraMake         |String         | Fabricante da câmera. Somente leitura.                                            |
|cameraModel        |String         | Modelo da câmera. Somente leitura.                                                   |
|exposureDenominator|Duplo         | O denominador da fração do tempo de exposição da câmera. Somente leitura. |
|exposureNumerator  |Duplo         | O numerador da fração do tempo de exposição da câmera. Somente leitura.   |
|fNumber            |Duplo         | O valor de f-stop da câmera. Somente leitura.                               |
|focalLength        |Double         | A distância focal da câmera. Somente leitura.                               |
|iso                |Int32          | O valor de ISO da câmera. Somente leitura.                                  |
|orientation        |Int16          | O valor da orientação da câmera. Gravável no OneDrive Personal.      |
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
