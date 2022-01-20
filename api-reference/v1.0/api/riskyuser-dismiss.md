---
title: 'riskyUser: dismiss'
description: Descartar um usuário arriscado
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f5ccfdc2fab1a4331a637ccc22ef7783c2721415
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088001"
---
# <a name="riskyuser-dismiss"></a>riskyUser: dismiss
Namespace: microsoft.graph

>**Observação:** Usar a API riskyUsers requer uma Azure AD Premium P2 de usuário.

Descartar o risco de um ou mais [objetos riskyUser.](../resources/riskyuser.md) Essa ação define o nível de risco do usuário direcionado como nenhum.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | IdentityRiskyUser.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | IdentityRiskyUser.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/dismiss
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|userIds|Coleção de cadeias de caracteres|Especifique os userIds a descartar no corpo da solicitação.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "riskyuser_dismiss"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/riskyuser-dismiss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/riskyuser-dismiss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/riskyuser-dismiss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/riskyuser-dismiss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/riskyuser-dismiss-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


