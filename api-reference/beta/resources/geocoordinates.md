---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: d49142ed414ad82ec149792e11e5a8c42d9837dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852637"
---
# <a name="geocoordinates-resource-type"></a>Tipo de recurso GeoCoordinates

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
