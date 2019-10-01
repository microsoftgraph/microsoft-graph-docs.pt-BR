---
author: JeremyKelley
description: O recurso GeoCoordinates fornece coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 86de97358591df8dc446b91d0be7a8192c7346f8
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333250"
---
# <a name="geocoordinates-resource-type"></a>tipo de recurso GeoCoordinates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
Se um [**driveItem**](driveitem.md) tiver uma faceta de **local** não nula, o item representará um arquivo com um local conhecido associada com ele.

> [!NOTE]
> Ao atualizar a latitude e a longitude de uma foto, um recurso de [foto](photo.md) (vazio ou ou outro) deve ser fornecido.

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição
|:----------|:-------|:--------------------------------------------------------
| altitude  | Duplo | Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.
| latitude  | Double | Opcional. A latitude, em valor decimal, para o item. Gravável no OneDrive Personal.
| longitude | Double | Opcional. A longitude, em valor decimal, para o item. Gravável no OneDrive Personal.

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

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": []
}
-->
