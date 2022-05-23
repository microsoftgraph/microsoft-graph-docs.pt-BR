---
title: 'cloudPCSnapshot: getSubscriptions'
description: Liste todas as assinaturas que podem ser usadas para armazenar um instantâneo ou instantâneos de um PC na nuvem para análise forense.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 879f6f6bfd382173958eca84a556571e58ae5f0b
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629244"
---
# <a name="get-cloudpcsubscription"></a>Obter cloudPcSubscription
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Liste todas as assinaturas [cloudPcSubscription](../resources/cloudpcsubscription.md) que podem ser usadas para armazenar um instantâneo ou instantâneos de um PC na nuvem para análise forense.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/virtualEndpoint/snapshots/getSubscriptions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e zero ou mais [objetos cloudPcSubscription](../resources/cloudpcsnapshot.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcsubscription"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/snapshots/getSubscriptions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcsubscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcsubscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcsubscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcsubscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-cloudpcsubscription-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcSubscription"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#cloudPcSubscriptions",
    "value":[
        {
            "subscriptionId": "8fd04a0b-ed49-46c0-a62d-e7980d829058",
            "subscriptionName":"Cloud PC Service INT"
        },
        {
            "subscriptionId": "618f7b25-b146-4c0e-a21b-2f1c67e78648",
            "subscriptionName":"Cloud PC HOBO Test1"
        }
    ]
}
```

