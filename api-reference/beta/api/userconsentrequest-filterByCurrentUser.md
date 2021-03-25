---
title: 'userConsentRequests: filterByCurrentUser'
description: Recupere userConsentRequests para o qual o usuário atual é o revistor.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ddef281b50a4a60895f141b433289a2fc3e8a1d3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201852"
---
# <a name="userconsentrequests-filterbycurrentuser"></a>userConsentRequests: filterByCurrentUser
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere [o userConsentRequests](../resources/userconsentrequest.md) para um appConsentRequest para o qual o usuário atual é o revistor e o status do userConsentRequest é `InProgress` .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|ConsentRequest.Read.All, ConsentRequest.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|ConsentRequest.Read.All, ConsentRequest.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>Parâmetros de função
Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|on|consentRequestFilterByCurrentUserOptions|Filtrar para consultar userConsentRequests para um appConsentRequest para o qual o usuário atual é um revistor. O valor permitido é `reviewer` . Obrigatório.|

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Essa função dá suporte ao  `$filter` parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) no corpo da resposta.

## <a name="example-list-all-userconsentrequests-for-which-the-current-user-is-the-reviewer-and-the-status-is-completed"></a>Exemplo: listar todos os userConsentRequests para os quais o usuário atual é o revistor e o status é Concluído

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')?$filter= (status eq 'Completed')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userConsentRequest)",
    "@odata.count": 1,
    "value": [
      {
      "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "reason": "I need access",
      "status": "Completed",
      "createdDateTime": "2019-10-18T19:07:19.7374554Z",
      "createdBy": {
        "user": {
          "id": "db60ab61-caea-4889-a824-98de31ef31b5",
          "displayName": "Alex Wilber",
          "userPrincipalName": "AlexW@contoso.com",
          "mail": "AlexW@contoso.com"
        }
      },
      "approval@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
      "approval": {
        "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
        "steps@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/steps",
        "steps": [
          {
            "id": "f5a4ca4a-1316-4872-8112-993c55dab51e",
            "displayName": null,
            "reviewedDateTime": "2019-10-19T04:12:09.633Z",
            "reviewResult": "Approve",
            "status": "Completed",
            "assignedToMe": true,
            "justification": "Admin consent granted.",
            "reviewedBy": {
              "id": "00000001-0000-0000-c000-000000000000",
              "displayName": "",
              "userPrincipalName": "",
              "mail": ""
            }
          }
        ]
      },
      "approvalId": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "completedDateTime": null,
      "customData": null
    }
  ]
}
```
