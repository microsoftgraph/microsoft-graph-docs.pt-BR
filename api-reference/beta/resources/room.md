---
title: tipo de recurso room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1599d029987be2cac8ac33b007dab485bc1474a4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154247"
---
# <a name="room-resource-type"></a>tipo de recurso room

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma sala em um locatário. 

No Exchange Online, cada sala é associada a uma caixa de correio de sala. Derivado do [local.](place.md)

## <a name="methods"></a>Métodos

| Método                              | Tipo de retorno                  | Descrição |
|:------------------------------------|:-----------------------------|:--------|
| [Listar locais](../api/place-list.md) | Uma coleção do tipo de local [](place.md) solicitado derivado | Obter uma coleção do tipo especificado de objeto **de** local definido no locatário. Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário. |
| [Obter local](../api/place-get.md)    | O tipo de local [](place.md) solicitado derivado            | Obter as propriedades e as relações do objeto **de local** especificado, como uma sala. |

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo                                              | Descrição |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | O endereço da sala. |
| audioDeviceName        | String                                            | Especifica o nome do dispositivo de áudio na sala. |
| bookingType            | [bookingType](#bookingtype-values)                | Tipo de sala. Os valores possíveis `standard` são `reserved` e. |
| building               | String                                            | Especifica o nome do edifício ou o número do edifício em que a sala está. |
| capacity               | Int32                                             | Especifica a capacidade da sala. |
| displayName            | String                                            | O nome associado à sala. |
| displayDeviceName      | String                                            | Especifica o nome do dispositivo de exibição na sala. |
| emailAddress           | String                                            | Endereço de email da sala. |
| floorLabel             | String                                            | Especifica um rótulo descritivo para o piso, por exemplo, P. |
| floorNumber            | Int32                                             | Especifica o número do piso em que a sala está. |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | Especifica o local da sala em coordenadas de latitude, longitude e, opcionalmente, altitude. |
| id                     | String                                            | Identificador exclusivo da sala. Somente leitura. |
| isWheelChairAccessible | Boolean                                           | Especifica se a sala é acessível para acessibilidade. |
| rótulo                  | String                                            | Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome. |
| nickname               | String                                            | Especifica um apelido para a sala, por exemplo, "conf room". |
| phone                  | Cadeia de caracteres                                            | O número de telefone da sala. |
| tags                   | Coleção de cadeias de caracteres                                 | Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou o tipo de móveis. |
| videoDeviceName        | String                                            | Especifica o nome do dispositivo de vídeo na sala. |

### <a name="bookingtype-values"></a>valores de bookingType

| Valor    | Descrição                                               |
|:---------|:----------------------------------------------------------|
| padrão | A sala pode ser reservada com base nas outras configurações deste cmdlet. Esse é o valor padrão. |
| reservado | A sala só está disponível por vir, primeiro a ser servido. Ele não pode ser reservado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": 1024,
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelChairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


