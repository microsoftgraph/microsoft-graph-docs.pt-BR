---
title: Obter authenticationListener
description: Leia as propriedades e os relacionamentos de um objeto authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3e6f07ac59e143ab7e9723c5a5b81a4c8489e54
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872419"
---
# <a name="get-authenticationlistener"></a>Obter authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o [authenticationListener especificado definido](../resources/authenticationlistener.md) para o evento onSignupStart no pipeline de autenticação.

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
GET /identity/events/onSignupStart/{id}
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

Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [authenticationListener](../resources/authenticationlistener.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-an-authenticationlistener-by-id"></a>Exemplo 1: Obter um authenticationListener por id

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
   }
}
```

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a>Exemplo 2: Expandir invokeUserFlowListener para uma authenticationListener específica

O exemplo a seguir obtém o ouvinte pela id do evento onSignupStart e expande o fluxo de usuário que é invocado.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invokeUserFlowListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
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
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationListener",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
