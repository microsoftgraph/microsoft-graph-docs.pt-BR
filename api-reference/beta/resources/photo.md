---
author: JeremyKelley
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6713e66b5ca14cfa6605b9e67d4bec152a321f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009220"
---
# <a name="photo-resource-type"></a>Tipo de recurso Photo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo           | Descrição
|:------------------------|:---------------|:----------------------------------
| **takenDateTime**       | DateTimeOffset | Representa a data e a hora em que a foto foi tirada. Somente leitura.
| **cameraMake**          | String         | Fabricante da câmera. Somente leitura.
| **cameraModel**         | String         | Modelo da câmera. Somente leitura.
| **fNumber**             | Duplo         | O valor de f-stop da câmera. Somente leitura.
| **exposureDenominator** | Duplo         | O denominador da fração do tempo de exposição da câmera. Somente leitura.
| **exposureNumerator**   | Duplo         | O numerador da fração do tempo de exposição da câmera. Somente leitura.
| **focalLength**         | Double         | A distância focal da câmera. Somente leitura.
| **iso**                 | Int64          | O valor de ISO da câmera. Somente leitura.

## <a name="remarks"></a>Comentários
O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
