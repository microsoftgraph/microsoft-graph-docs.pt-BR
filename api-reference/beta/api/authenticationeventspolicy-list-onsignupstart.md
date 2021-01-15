---
title: Listar ouvintes onSignUpStart
description: Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 346db0f1085190252b2bb8e48dcfcb8adfc23f61
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872363"
---
# <a name="list-onsignupstart-listeners"></a>Listar ouvintes onSignUpStart

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart. O evento onSignUpStart dá suporte ao [tipo invokeUserFlowListener.](../resources/invokeuserflowlistener.md)

Quando um [invokeUserFlowListener](../resources/invokeuserflowlistener.md) é atribuído [a](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) um evento onSignUpStart, um aplicativo é associado a um fluxo de usuário, habilitando um processo de inscrição de autoatendente nele. Depois que o evento de autenticação para invocar um fluxo de usuário é criado, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte `$expand` ao parâmetro de consulta OData para expandir os detalhes de um invokeUserFlowListener. Veja abaixo um exemplo. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos authenticationListener](../resources/authenticationlistener.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-authenticationlisteners-for-the-onsignupstart-event"></a>Exemplo 1: Listar authenticationListeners para o evento onSignUpStart

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.authenticationListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      }
    },
    {
      "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
          "includeApplications": [
              "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      }
    }
  ]
}
```

### <a name="example-2-expand-invokeuserflowlisteners-in-authenticationlisteners-for-the-onsignupstart-event"></a>Exemplo 2: Expandir invokeUserFlowListeners em authenticationListeners para o evento onSignUpStart

O exemplo a seguir lista os ouvintes definidos para o evento onSignupStart e, para cada ouvinte, expande o fluxo do usuário invocado.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart?$expand=microsoft.graph.invokeUserFlowListener/userFlow
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.invokeUserFlowListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    },
    {
      "@odata.type": "#microsoft.graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
        "includeApplications": [
            "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List onSignUpStart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
