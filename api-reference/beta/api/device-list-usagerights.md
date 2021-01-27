---
title: Listar usageRights do dispositivo
description: Recupere uma lista de objetos usageRights para um dispositivo.
author: jeeshnair
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 73a67ecd46085c7c4369e68db5f72655cbaf395a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013608"
---
# <a name="list-device-usagerights"></a>Listar usageRights do dispositivo
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos usageRight](../resources/usageright.md) para um determinado dispositivo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /devices/{objectId}/usageRights
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Essa API dá suporte ao $filter [de consulta OData.](/graph/query-parameters) Os seguintes padrões de $filter são suportados:

- $filter = state eq 'value'
- $filter = serviceIdentifier eq 'value'
- $filter = state eq 'value' and serviceIdentifier eq 'value'
- $filter = estado em ('value1', 'value2')
- $filter = serviceIdentifier em ('value1', 'value2')
- $filter = estado em ('value1', 'value2') e serviceIdentifier em ('value1', 'value2')

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|odata.maxpagesize|Definir a pereferência do tamanho máximo da página de resultados. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção [de objetos usageRight](../resources/usageright.md) no corpo da resposta.

Além disso, se houver mais páginas na resposta, um @odata.nextLink será retornado.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-all-usage-rights-for-a-device"></a>Exemplo 1: Obter todos os direitos de uso de um dispositivo
 
#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/devices/fead5c35-ebc5-47c4-a909-c43b4faf2160/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "99f828b9-09f2-445d-a758-b6727316dbe1",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-device-with-specific-service-identifiers-and-states"></a>Exemplo 2: Obter direitos de uso para um dispositivo com identificadores de serviço e estados específicos

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "value": [
    {
      "id": "9905e6b1-9040-4926-b028-fdb748c359d6",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
