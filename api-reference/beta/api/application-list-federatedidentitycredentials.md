---
title: Listar federatedIdentityCredentials
description: Obter uma lista dos objetos federatedIdentityCredential e suas propriedades.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 468d5668c90406448102e05f7ba1386865e58145
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990908"
---
# <a name="list-federatedidentitycredentials"></a>Listar federatedIdentityCredentials
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [objetos federatedIdentityCredential](../resources/federatedidentitycredential.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.Read.All, Application.ReadWrite.All    |
|Delegada (conta pessoal da Microsoft) |  Application.ReadWrite.All |
|Aplicativo | Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /applications/{applicationsId}/federatedIdentityCredentials
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos parâmetros de consulta ( ) e OData para `$filter` ajudar a personalizar a `eq` `$select` [](/graph/query-parameters) resposta. Por exemplo, `/applications/{id}/federatedIdentityCredentials?$filter=subject eq 'value'`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos federatedIdentityCredential](../resources/federatedidentitycredential.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_federatedidentitycredential"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-federatedidentitycredential-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-federatedidentitycredential-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-federatedidentitycredential-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-federatedidentitycredential-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-federatedidentitycredential-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.federatedIdentityCredential)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.id": "https://graph.microsoft.com/v2/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/directoryObjects/$/Microsoft.DirectoryServices.Application('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/bdad0963-4a7a-43ae-b569-e67e1da3f2c0",
      "id": "bdad0963-4a7a-43ae-b569-e67e1da3f2c0",
      "name": "testing",
      "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
      "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
      "description": "This is my test  federated identity credential 03",
      "audiences": [
          "api://AzureADTokenExchange"
      ]
    }
  ]
}
```

