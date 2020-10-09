---
title: Listar b2xIdentityUserFlows
description: Recupere uma lista de objetos b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 085b75ae496ba785822c00a9cda338d363e879be
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406269"
---
# <a name="list-b2xidentityuserflows"></a>Listar b2xIdentityUserFlows

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de objetos [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)|IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All|
|Delegado (conta pessoal da Microsoft)| Sem suporte.|
|Aplicativo|IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All|

A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:

* Administrador global
* Administrador de fluxo de usuário de identidade externa

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Você pode usar o `$expand` para expandir Propriedades de fluxo de usuário específicas que não são expandidas por padrão.

Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---------------|:----------|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-all-b2xidentityuserflow-objects"></a>Exemplo 1: listar todos os objetos b2xIdentityUserFlow

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
    ]
}
```

### <a name="example-2-list-all-b2xidentityuserflow-objects-and-expand-identityproviders"></a>Exemplo 2: listar todos os objetos b2xIdentityUserFlow e expandir identityProviders

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows?$expand=identityProviders
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows(identityProviders)",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List b2xUserFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_b2xUserFlows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_b2xUserFlows_expand/container/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


