---
author: JeremyKelley
description: O recurso geoCoordinates fornece coordenadas geográficas e elevação de um local com base nos metadados contidos no arquivo.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: e3b0ac4f616afe648b5c30dc9d15978036a7ab80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129419"
---
# <a name="geocoordinates-resource-type"></a>Tipo de recurso geoCoordinates

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece coordenadas geográficas e elevação de um local com base nos metadados contidos no arquivo.
Se um [**driveItem**](driveitem.md) tiver  uma faceta de local não nulo, o item representará um arquivo com um local conhecido com ele.

> [!NOTE]
> Ao atualizar a latitude e a longitude de uma foto, um recurso [de](photo.md) foto (vazio ou não) deve ser fornecido.

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição
|:----------|:-------|:--------------------------------------------------------
| altitude  | Double | Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.
| latitude  | Double | Opcional. A latitude, em valor decimal, para o item. Writable no OneDrive Personal.
| longitude | Double | Opcional. A longitude, em valor decimal, para o item. Writable no OneDrive Personal.

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


