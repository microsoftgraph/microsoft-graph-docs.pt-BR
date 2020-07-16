---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a62a138cbd48645b6b296abcde72af0cef19e259
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863730"
---
# <a name="photo-resource-type"></a>Tipo de recurso Photo

Namespace: microsoft.graph

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
  "orientation": 3,
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
| **iso**                 | Int32          | O valor de ISO da câmera. Somente leitura.
| **orientation**         | Int16          | O valor da orientação da câmera. Gravável no OneDrive Personal.      |

## <a name="remarks"></a>Comentários

O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
