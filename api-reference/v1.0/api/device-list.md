---
title: Listar dispositivos
description: Recupera uma lista de objetos de dispositivos registrados na organização.
author: sandeo-MSFT
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a6b538113c747c66f90f41447d34a1097e573f5b
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266212"
---
# <a name="list-devices"></a>Listar dispositivos

Namespace: microsoft.graph

Recupera uma lista de objetos de dispositivos registrados na organização.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Device.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método suporta aos parâmetros de consulta `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, e `$top` [OData](/graph/query-parameters) para ajudar a personalizar a resposta. Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       |  Descrição|
|:-----------|:------------|
| Autorização  | {token} de portador. Obrigatório. |
| ConsistencyLevel | eventualmente. Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-list-of-devices"></a>Exemplo 1: Obter uma lista de dispositivos

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-devices-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-devices"></a>Exemplo 2: Obter apenas uma contagem de dispositivos

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

>**Observação:** Os parâmetros e de consulta atualmente não estão `$count` `$search` disponíveis em locatários do Azure AD B2C.

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

294
```


### <a name="example-3-list-all-devices-and-return-only-their-id-and-extensionattributes-properties"></a>Exemplo 3: listar todos os dispositivos e retornar apenas suas propriedades id e extensionAttributes

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_devices_select"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$select=id,extensionAttributes
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices(id,extensionAttributes)",
    "value": [
        {
            "id": "6a59ea83-02bd-468f-a40b-f2c3d1821983",
            "extensionAttributes": {
                "extensionAttribute1": null,
                "extensionAttribute2": null,
                "extensionAttribute3": null,
                "extensionAttribute4": null,
                "extensionAttribute5": null,
                "extensionAttribute6": null,
                "extensionAttribute7": null,
                "extensionAttribute8": null,
                "extensionAttribute9": null,
                "extensionAttribute10": null,
                "extensionAttribute11": null,
                "extensionAttribute12": null,
                "extensionAttribute13": null,
                "extensionAttribute14": null,
                "extensionAttribute15": null
            }
        }
    ]
}
```


### <a name="example-4-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a>Exemplo 4: use $filter e $top para obter um dispositivo com um nome de exibição que comece com "a" incluindo uma contagem de objetos retornados

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

>**Observação:** Os parâmetros e de consulta atualmente não estão `$count` `$search` disponíveis em locatários do Azure AD B2C.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-a-count-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-5-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a>Exemplo 5: use $search para obter dispositivos com nomes de exibição que contenham as letras "Android", incluindo uma contagem de objetos retornados

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Essa solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual`, pois a solicitação tem `$search` e a cadeia de caracteres de consulta `$count=true`. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

>**Observação:** Os parâmetros e de consulta atualmente não estão `$count` `$search` disponíveis em locatários do Azure AD B2C.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-android-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-android-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-android-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-android-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-android-count-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-6-get-device-using-filter-on-extensionattributes"></a>Exemplo 6: Obter dispositivo usando filtro em extensionAttributes

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Essa solicitação requer o header **ConsistencyLevel** definido como e a cadeia de caracteres de consulta porque a propriedade `eventual` `$count=true` extensionAttributes oferece suporte apenas a parâmetros de `$filter` consulta avançados. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

>**Observação:** Os parâmetros e de consulta atualmente não estão `$count` `$search` disponíveis em locatários do Azure AD B2C.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_by_extensionAttribute"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=extensionAttributes/extensionAttribute1 eq 'BYOD-Device'&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-by-extensionattribute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-by-extensionattribute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-by-extensionattribute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-by-extensionattribute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-devices-by-extensionattribute-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
    "@odata.count": 1,
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/6a59ea83-02bd-468f-a40b-f2c3d1821983/Microsoft.DirectoryServices.Device",
            "id": "6a59ea83-02bd-468f-a40b-f2c3d1821983",
            "accountEnabled": true,
            "approximateLastSignInDateTime": "2021-10-21T06:36:56Z",
            "createdDateTime": "2021-09-21T15:16:30Z",
            "deviceId": "eab73519-780d-4d43-be6d-a4a89af2a348",
            "displayName": "DESKTOP-LK3PESR",
            "operatingSystem": "Windows",
            "operatingSystemVersion": "10.0.19043.1237",
            "physicalIds": [],
            "extensionAttributes": {
                "extensionAttribute1": "BYOD-Device",
                "extensionAttribute2": null,
                "extensionAttribute3": null,
                "extensionAttribute4": null,
                "extensionAttribute5": null,
                "extensionAttribute6": null,
                "extensionAttribute7": null,
                "extensionAttribute8": null,
                "extensionAttribute9": null,
                "extensionAttribute10": null,
                "extensionAttribute11": null,
                "extensionAttribute12": null,
                "extensionAttribute13": null,
                "extensionAttribute14": null,
                "extensionAttribute15": null
            },
            "alternativeSecurityIds": [
                {
                    "type": 2,
                    "identityProvider": null,
                    "key": "WAA1ADAAOQA6AD...QBnAD0A"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- 
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
