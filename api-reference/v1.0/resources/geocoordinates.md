---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: O recurso GeoCoordinates fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 048fefc8938a789a0aae06f3dd6f50c25c305c31
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130505"
---
# <a name="geocoordinates-resource-type"></a>Tipo de recurso GeoCoordinates

Namespace: microsoft.graph

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
| altitude  | Double | Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.
| latitude  | Double | Opcional. A latitude, em valor decimal, para o item. Somente leitura.
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

