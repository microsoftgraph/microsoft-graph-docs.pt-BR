---
title: tipo de recurso RoomList
description: Representa um grupo de salas criadas pela empresa.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f0c56f986663c71d8c6817c0024919e8714af94a
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841252"
---
# <a name="roomlist-resource-type"></a>tipo de recurso RoomList

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo de objetos [Room](room.md) definidos no locatário.

Derivado do [local](place.md).

## <a name="methods"></a>Métodos

| Método                              | Tipo de retorno                  | Descrição |
|:------------------------------------|:-----------------------------|:--------|
| [Locais de lista](../api/place-list.md) | Uma coleção do tipo de [local](place.md) solicitado e derivado | Obtém uma coleção do tipo especificado do objeto **Place** definido no locatário. Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário.|
| [Obter local](../api/place-get.md)    | O tipo de [local](place.md) solicitado e derivado            | Obtenha as propriedades e os relacionamentos do objeto **local** especificado, como uma lista de salas. |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                              | Descrição |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | O endereço da lista de salas. |
| displayName    | String                                            | O nome associado à lista de salas. |
| emailAddress   | String                                            | O endereço de email da lista de salas. |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | Especifica o local da sala de opções no latitude, longitude e (opcionalmente) as coordenadas de altitude. |
| id             | String                                            | Identificador exclusivo da lista de salas. Somente leitura. |
| phone          | Cadeia de caracteres                                            | O número de telefone da lista de salas. |

## <a name="relationships"></a>Relações

| Relação | Tipo                         | Descrição          |
|:-------------|:-----------------------------|:---------------------|
| quartos        | [colocar](place.md) coleção | Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
