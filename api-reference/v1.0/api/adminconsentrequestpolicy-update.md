---
title: Atualizar adminConsentRequestPolicy
description: Atualize as propriedades de um objeto adminConsentRequestPolicy.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2cc16ba867e5084814565201d8ad8d056fd1dc37
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996809"
---
# <a name="update-adminconsentrequestpolicy"></a>Atualizar adminConsentRequestPolicy

Namespace: microsoft.graph

Atualize as propriedades de [um objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.ReadWrite.ConsentRequest, Directory.ReadWrite.All|

Ao chamar em nome de um usuário, o usuário precisa pertencer à função de diretório [Administrador Global.](/azure/active-directory/roles/permissions-reference)

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)

A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Especifica se o recurso de solicitação de consentimento do administrador está habilitado ou desabilitado.|
|notifyReviewers|Boolean|Especifica se os revisadores receberão notificações.|
|remindersEnabled|Booliano|Especifica se os revisadores receberão emails de lembrete.|
|requestDurationInDays|Int32|Especifica a duração em que a solicitação está ativa antes de expirar automaticamente se nenhuma decisão for aplicada.|
|revisadores|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|A lista de revisadores para o consentimento do administrador.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `204 No content` [objeto adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy 
Content-Type: application/json

{
  "isEnabled": true,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "query": "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
      "queryType": "MicrosoftGraph"
    },
    {
      "query": "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
      "queryType": "MicrosoftGraph"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-adminconsentrequestpolicy-go-snippets.md)]
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
Content-Type: text/plain
```
