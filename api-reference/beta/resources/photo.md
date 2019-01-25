---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
ms.openlocfilehash: 91b893fe3d6c78e3c3e16cbc41c7d7543b08f8d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527623"
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
| **fNumber**             | Double         | O valor de f-stop da câmera. Somente leitura.
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
  "suppressions": [
    "Error: /api-reference/beta/resources/photo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
