---
title: Obter local
description: Recupere as propriedades e os relacionamentos de um objeto local.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0dc07c3c649cb472abc2a33a819fcaf9a7935589
ms.sourcegitcommit: b88dce7297f196345f16c2c126d7bdd482d22a23
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/02/2020
ms.locfileid: "44006318"
---
# <a name="get-place"></a>Obter local

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Obtenha as propriedades e os relacionamentos de um objeto [local](../resources/place.md) especificado por sua ID ou endereço de email. 

O objeto **local** pode ser um dos seguintes tipos:

* Uma [sala](../resources/room.md) que inclui Propriedades sofisticadas, como um endereço de email para a sala, e suporte à acessibilidade, capacidade e dispositivo.
* Uma [lista de salas](../resources/roomlist.md) que inclui um endereço de email para a lista de salas e uma propriedade de navegação para obter a coleção de instâncias de **sala** na lista de salas.

A **sala** e a **salalist** são derivadas do objeto [local](../resources/place.md) . 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Place.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte |
| Aplicativo                            | Place.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Use $select para obter propriedades de **local** específico.

Para obter mais informações sobre opções de consulta OData, confira [parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [local](../resources/place.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-room"></a>Exemplo 1: obter uma sala
#### <a name="request"></a>Solicitação

O exemplo a seguir especifica a **ID** de uma **sala** para obter suas propriedades.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "name": "get_room",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
    "@odata.type": "#microsoft.graph.room",
    "id": "3162F1E1-C4C0-604B-51D8-91DA78989EB1",
    "emailAddress": "cf100@contoso.com",
    "displayName": "Conf Room 100",
    "address": {
      "street": "4567 Main Street",
      "city": "Buffalo",
      "state": "NY",
      "postalCode": "98052",
      "countryOrRegion": "USA"
    },
    "geoCoordinates": {
      "latitude": 47.640568390488626,
      "longitude": -122.1293731033803
    },
    "phone": "000-000-0000",
    "nickname": "Conf Room",
    "label": "100",
    "capacity": "50",
    "building": "1",
    "floorNumber": 1,
    "isManaged": true,
    "isWheelchairAccessible": false,
    "bookingType": "standard",
    "tags": [
      "bean bags"
    ],
    "audioDeviceName": null,
    "videoDeviceName": null,
    "displayDevice": "surface hub"
}
```

### <a name="example-2-get-a-room-list"></a>Exemplo 2: obter uma lista de salas
#### <a name="request"></a>Solicitação

O exemplo a seguir especifica o **EmailAddress** de uma **RoomList** para obter suas propriedades.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "name": "get_roomlist",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
  "@odata.type": "#microsoft.graph.roomList",
  "id": "DC404124-302A-92AA-F98D-7B4DEB0C1705",
  "displayName": "Building 1",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geocoordinates": null,
  "phone": null,
  "emailAddress": "bldg1@contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
