---
title: tipo de recurso de sala
description: Especifica as propriedades de uma sala em um locatário.
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d676dbcd36760bc14edb38b35f6f93573f03b9b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117771"
---
# <a name="room-resource-type"></a>tipo de recurso de sala

Namespace: microsoft.graph

Representa uma sala em um locatário. 

Em Exchange Online, cada sala é associada a uma caixa de correio de sala. Derivado do [local](place.md).

## <a name="methods"></a>Métodos

| Método                              | Tipo de retorno                  | Descrição |
|:------------------------------------|:-----------------------------|:--------|
| [Listar locais](../api/place-list.md) | Uma coleção do tipo de local solicitado e [derivado](place.md) | Obter uma coleção do tipo especificado de **objeto place** definido no locatário. Por exemplo, você pode obter todas as salas, todas as listas de salas ou as salas em uma lista de salas específica no locatário. |
| [Obter lugar](../api/place-get.md)    | O tipo de local [](place.md) solicitado e derivado            | Obter as propriedades e as relações do objeto **local** especificado, como uma sala. |

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo                                              | Descrição |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | O endereço da sala. |
| audioDeviceName        | String                                            | Especifica o nome do dispositivo de áudio na sala. |
| bookingType            | [bookingType](#bookingtype-values)                | Tipo de sala. Os valores possíveis `standard` são e `reserved` . |
| building               | String                                            | Especifica o nome do edifício ou o número de construção em que a sala está. |
| capacity               | Int32                                             | Especifica a capacidade da sala. |
| displayName            | Cadeia de caracteres                                            | O nome associado à sala. |
| displayDeviceName      | String                                            | Especifica o nome do dispositivo de exibição na sala. |
| emailAddress           | String                                            | Endereço de email da sala. |
| floorLabel             | Cadeia de caracteres                                            | Especifica um rótulo descritivo para o piso, por exemplo, P. |
| floorNumber            | Int32                                             | Especifica o número do piso em que a sala está. |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | Especifica o local da sala em latitude, longitude e, opcionalmente, coordenadas de altitude. |
| id                     | String                                            | Identificador exclusivo da sala. Somente leitura. |
| isWheelChairAccessible | Booliano                                           | Especifica se a sala está acessível para cadeira de rodas. |
| rótulo                  | Cadeia de caracteres                                            | Especifica um rótulo descritivo para a sala, por exemplo, um número ou nome. |
| nickname               | Cadeia de caracteres                                            | Especifica um apelido para a sala, por exemplo, "conf room". |
| phone                  | Cadeia de caracteres                                            | O número de telefone da sala. |
| categorias                   | Coleção String                                 | Especifica recursos adicionais da sala, por exemplo, detalhes como o tipo de exibição ou tipo de móvel. |
| videoDeviceName        | String                                            | Especifica o nome do dispositivo de vídeo na sala. |

### <a name="bookingtype-values"></a>valores bookingType

| Valor    | Descrição                                               |
|:---------|:----------------------------------------------------------|
| standard | A sala está disponível e pode ser reservada. Esse é o valor padrão. |
| reservado | A sala está disponível somente por primeira vez, primeiro servido. Não é possível reservá-lo.|

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

