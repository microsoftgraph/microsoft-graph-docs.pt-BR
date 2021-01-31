---
title: tipo de recurso room
description: Especifica as propriedades de uma sala em um locatário.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1a297888d8b469944b5fdbebaa9948db0ba59c97
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059662"
---
# <a name="room-resource-type"></a>tipo de recurso room

Namespace: microsoft.graph

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
| audioDeviceName        | Cadeia de caracteres                                            | Especifica o nome do dispositivo de áudio na sala. |
| bookingType            | [bookingType](#bookingtype-values)                | Tipo de sala. Os valores possíveis `standard` são e `reserved` . |
| building               | Cadeia de caracteres                                            | Especifica o nome do edifício ou o número do edifício em que a sala está. |
| capacity               | Int32                                             | Especifica a capacidade da sala. |
| displayName            | Cadeia de caracteres                                            | O nome associado à sala. |
| displayDeviceName      | Cadeia de caracteres                                            | Especifica o nome do dispositivo de exibição na sala. |
| emailAddress           | String                                            | Endereço de email da sala. |
| floorLabel             | Cadeia de caracteres                                            | Especifica um rótulo descritivo para o piso, por exemplo, P. |
| floorNumber            | Int32                                             | Especifica o número do piso em que a sala está. |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | Especifica o local da sala em coordenadas de latitude, longitude e, opcionalmente, altitude. |
| id                     | Cadeia de caracteres                                            | Identificador exclusivo da sala. Somente leitura. |
| isWheelChairAccessible | Booliano                                           | Especifica se a sala é acessível para acessibilidade. |
| rótulo                  | Cadeia de caracteres                                            | Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome. |
| nickname               | Cadeia de caracteres                                            | Especifica um apelido para a sala, por exemplo, "conf room". |
| phone                  | Cadeia de caracteres                                            | O número de telefone da sala. |
| tags                   | Coleção de cadeias de caracteres                                 | Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou o tipo de móveis. |
| videoDeviceName        | Cadeia de caracteres                                            | Especifica o nome do dispositivo de vídeo na sala. |

### <a name="bookingtype-values"></a>valores de bookingType

| Valor    | Descrição                                               |
|:---------|:----------------------------------------------------------|
| padrão | A sala está disponível e pode ser reservada. Esse é o valor padrão. |
| reservado | A sala só está disponível por vir, primeiro a ser servido. Ele não pode ser reservado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
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

