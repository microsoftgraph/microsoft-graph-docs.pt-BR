---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: cafd9d72e6c7959b32672744959393ae9478c5b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558073"
---
# <a name="geocoordinates-resource-type"></a>Tipo de recurso GeoCoordinates

O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição
|:----------|:-------|:--------------------------------------------------------
| altitude  | Duplo | Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.
| latitude  | Duplo | Opcional. A latitude, em valor decimal, para o item. Somente leitura.
| longitude | Double | Opcional. A longitude, em valor decimal, para o item. Somente leitura.

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
