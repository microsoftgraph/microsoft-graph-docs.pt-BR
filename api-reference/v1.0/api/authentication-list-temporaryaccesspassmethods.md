---
title: Listar temporaryAccessPassMethods
description: Obtenha uma lista dos objetos temporaryAccessPassAuthenticationMethod para um usuário.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0778843b50520d6d2f5ef73844fc58853e8e428f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438519"
---
# <a name="list-temporaryaccesspassmethods"></a>Listar temporaryAccessPassMethods
Namespace: microsoft.graph

Recupere uma lista dos objetos [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) de um usuário e suas propriedades. Essa API retornará apenas um único objeto na coleção, pois um usuário pode ter apenas um método de Passagem de Acesso Temporário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Permissões agindo por conta próprio

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

### <a name="permissions-acting-on-other-users"></a>Permissões que atuam em outros usuários

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:---------------------------------------|:-------------------------|
| Delegada (conta corporativa ou de estudante)     | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |


Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Administrador global
* Leitor global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request"></a>Solicitação 
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método `200 OK` retorna um código de resposta e uma coleção de objetos [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.  Essa chamada retornará apenas um único objeto porque apenas um **temporaryAccessPassAuthenticationMethod** pode ser definido nos usuários.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-temporaryaccesspassauthenticationmethod-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-temporaryaccesspassauthenticationmethod-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('071cc716-8147-4397-a5ba-b2105951cc0b')/authentication/temporaryAccessPassMethods",
     "value": [
        {
            "id": "bdaede67-61e0-4349-9347-d2d6afd84009",
            "temporaryAccessPass": null,
            "createdDateTime": "2022-06-06T16:43:04.6438213Z",
            "startDateTime": "2022-06-06T16:48:03.027Z",
            "lifetimeInMinutes": 60,
            "isUsableOnce": false,
            "isUsable": false,
            "methodUsabilityReason": "NotYetValid"
        }
    ]
}
```
