---
title: Listar unifiedGroupSources do guardião
description: Obtenha uma lista dos objetos unifiedGroupSource do guardião e suas propriedades.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e2cd4de401e37e4616af2a53f4abf18e9b2b205c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094954"
---
# <a name="list-custodians-unifiedgroupsources"></a>Listar unifiedGroupSources do guardião
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos unifiedGroupSource](../resources/security-unifiedgroupsource.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e uma coleção de [objetos unifiedGroupSource](../resources/security-unifiedgroupsource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedgroupsource"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/unifiedGroupSources
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedgroupsource-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.unifiedGroupSource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/groups/32e14fa4-3106-4bd2-a245-34bf0c718a7e",
            "displayName": "Design (Mailbox)",
            "createdDateTime": "2022-05-23T02:35:42.926309Z",
            "holdStatus": "applied",
            "id": "32e14fa4-3106-4bd2-a245-34bf0c718a7e",
            "includedSources": "mailbox,site",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            },
            "group": {
                "email": "Design@M365x809305.onmicrosoft.com",
                "webUrl": "https://m365x809305.sharepoint.com/sites/Design",
                "id": "32e14fa4-3106-4bd2-a245-34bf0c718a7e",
                "displayName": "Design (Mailbox)",
                "createdDateTime": "2022-05-23T02:35:42.926309Z"
            }
        },
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/groups/21be9868-b58b-4f8b-800c-591e9ad8d4ec",
            "displayName": "CEO Connection (Mailbox)",
            "createdDateTime": "2022-05-23T02:35:42.926309Z",
            "holdStatus": "applied",
            "id": "21be9868-b58b-4f8b-800c-591e9ad8d4ec",
            "includedSources": "mailbox,site",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            },
            "group": {
                "email": "ceoconnection@M365x809305.onmicrosoft.com",
                "webUrl": "https://m365x809305.sharepoint.com/sites/ceoconnection",
                "id": "21be9868-b58b-4f8b-800c-591e9ad8d4ec",
                "displayName": "CEO Connection (Mailbox)",
                "createdDateTime": "2022-05-23T02:35:42.926309Z"
            }
        }
    ]
}
```

